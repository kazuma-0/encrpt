# Encrpt
A password manager with TOTP Integration( on development ).

## Tools Used
 - `Python` was used for the backend as an api. It handles the database management and encryption.
 - `React JS` was used for the frontend with a clean UserInterface.
 
 ### How it works
 The backend uses Flask, sqlite3 and cryptography to handle data, encrypt them and add them to the database. 
 Frontend handles all the actions like adding new entries, managing passwords, etc.
 whenever a authorised user who has the token add a new entry, it is then encrypted using the cryptography module.
 Then the key which is over 44 characters in length is either mailed or send to them using webhooks, whenever the user wants the password 
 they can use the key to get the password. Only authorised users with a user authication code which is 20 or more characters in length 
 can add new passwords or manage/view the passwords.
