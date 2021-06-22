# Easy-Passbolt
    
1. First of all edit the env directory files so the database and passbolt can connect and set the google mail conf (it can be any mail server). Remember to enable the less secure feature on the mail account if used with gmail.

2. Up the docker-compose file
    > docker-compose up -d
3. Execute changing the mail, name, and lastname.  
    >docker-compose exec passbolt su -m -c "/usr/share/php/passbolt/bin/cake passbolt register_user -u [user@mail.com] -f [fullname] -l [lastname] -r admin" -s /bin/sh www-data
4. Now open the link prompted on the terminal with any browser. Add the extension and set up the account. This will be the "Real Administrator" account. Where you will be able to manage users, groups and passwords.
5. Enjoy 😉