class employee:
    
    def _init_(self, firstname, lastname, salary):
        self.firstname = firstname
        self.lastname = lastname
        self.salary = salary
        self.email = self.firstname + "." + self.lastname + "@kite.com"
              
    def giveRaise(self, salary):
        self.salary = salary
        
class developer(employee):
    
    def _init_(self, firstname, lastname, salary, programming_languages):
        super()._init_(firstname, lastname, salary)
        self.prog_langs = programming_languages
        
    def addLanguage(self, lang):
        self.prog_langs += [lang]
        
employee1 = employee("John", "Smith", 80000)

print(employee1.salary)

employee1.giveRaise(10000)

print(employee1.salary)

dev1 = developer("Talor", "Levy", 115000, ["Python", "Java"])

print(dev1.salary)

dev1.giveRaise(20000)

print(dev1.salary)

dev1.addLanguage("SQL")

print(dev1.prog_langs)
