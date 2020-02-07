# This doc explain how to setup relay agent to send mail if we have access to smtp Server.

1. yum install postfix
2. make below change to "/etc/postfix/main.cf"
  relayhost = mail.smganalytics.com:25
3. systemctl restart postfix
4. systemctl enable postfix

#Hurray!!. Thats all now you can send mail 

Example:
echo "Subject: hello" | sendmail -v acmeofmanas@gmail.com
