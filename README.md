# Password-Manager-using-Mysql-and-AES

1. All the codes can be found and executed in the "codes" Folder file. Just running the codes will do.

2. All the code files(2 languages) are in the "Codes" folder.

Table of contents:
1. Prerequisites
2. Setup
3. Running the codes

1. Prerequisites
•	MySQL installed
•	openssl installed
•	Matlab installed 
•	Python installed


2. Setup
->Connect the MySQL database to Python using MySQL connecter library.
->give your proper credentials of mysql database in python server code to connecting to mysql database.
->And create a database named pm_ap and a table named passwords in mysql workbench.


->In python,Running the Server.py and use your system's ip address and socket number is 5000 to connect to server as a client and you can save your passwords without a worry.
->index.hmtl is the template used for gui
->make sure to change the path for certificate and key in the python code.
   In matlab only AES was implemented.

**** NOTE :Points Discussed During Presentation.
->Here we are using mysql database to store passwords so our data wont be lost once server is down.
->We are using HTTPs using a self generated certificate and key using openssl(in the browser it may show that our server is not secure because our certificate is not authorised by a certifying authority but still communication is secure)
->there is no user distinction because we can save any number of entries in the database with same domain and since there will different key for decrypting each user will get their own saved password.
->even if database password is compromised we are only saving hash of the master password in the database and we use original master password for decrypting and encrypting, we are saving hash of the master password for veryfing the hash of master password given by user for retrieving passwords.

 
----------------------------------------------------------------------------------------------------------------------------


****please make sure to install all the libraries used in the python code.
