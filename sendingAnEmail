# import the EmailMessage, ssl, and smtp libraries

from email.message import EmailMessage
import ssl
import smtplib


# specify the email login credentials and the receiver

email_sender = 'talorlevy26@gmail.com'
email_password = 'rzagexrqgesndych'
email_receiver = 'talorlv123@hotmail.com'


# create the subject and body of the email

subject = "Check This Email!"
body = """
This is the test body of the email! I could say all kinds of weird, fantastic things. Like... OOGABOOGABOOGA!!!
"""


# create an email instance via the EmailMessage library

em = EmailMessage()
em['From'] = email_sender
em['To'] = email_receiver
em['Subject'] = subject
em.set_content(body)


# establish context via the SSL library to be used in conjunction with the SMTP protocol to send the email

context = ssl.create_default_context()


# send the email via the SMTP library using all the info created/collected before line 39!

with smtplib.SMTP_SSL('smtp.gmail.com', 465, context=context) as smtp:
    smtp.login(email_sender, email_password)
    smtp.sendmail(email_sender, email_receiver, em.as_string())

