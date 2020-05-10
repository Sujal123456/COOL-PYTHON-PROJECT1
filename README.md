# COOL-PYTHON-PROJECT1
EMAIL AUTOMATION USING PYTHON




import smtplib
from email.mime.multipart import MIMEMultipart
from email.mime.multipart import MIMEText


from_addr= 'sujalmaiti123456@gmail.com'
to.addr= ['sujalmaiti97@gmail.com']
msg=MIMEMultipart()
msg['To']=",".join(to_addr)
msg['subject']= 'just to check'
body='hello world'
msg.attach(MIMEText(body,'plain'))
email=""
password=""
mail=smtplib.SMIP('setp.gmail.com',587)
mail.ehlo()
mail.start.ls()
mail.login(email,password)
text=msg.as_string()
mail.sendmail(from_addr,to_addr,text)
mail.quit()
