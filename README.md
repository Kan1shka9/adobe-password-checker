# 📇 Adobe Password Checker 🔑

Combined list hint+passwords from: 
  - [``adobe-top100.txt``](http://stricture-group.com/files/adobe-top100.txt)
  - [``adobe_sanitized_passwords_with_bad_hints.txt``](http://web.mit.edu/zyan/Public/adobe_sanitized_passwords_with_bad_hints.txt)
  
###### Usage

```sh
$ grep "@yahoo.com" cred > hashlist.txt
```

  - Replace 

    - ``yahoo.com`` with domain being pen-tested
    - ``cred`` with the file name of the publically leaked password/hashdump file

```sh
$ git clone https://github.com/Kan1shka9/adobe-password-checker.git /opt/adobe-password-checker
$ mv hashlist.txt /opt/adobe-password-checker
$ cd /opt/adobe-password-checker
$ ls
foundpw.csv  hashlist.txt  password_check.py  README.md
$ python password_check.py
```

- Use the credentials to login to Outlook Web Access (OWA) and against VPN logins
- Use email address for spear phishing
