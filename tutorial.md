# This is the step-by-step guide and instructions on how to install and configure DVWA in Kali Linux.
    NOTE: If you are looking for the main project content, it is located in the main.md file of this repository.
#
1.  Go to https://github.com/digininja/DVWA and clone the HTTPS code link. Please follow the terminal commands.

![1 1](https://github.com/user-attachments/assets/ef5b0b4c-4e5b-447c-ae3f-d34020e6f684)
#
![1 2](https://github.com/user-attachments/assets/6bdd316e-c629-4edc-9abf-32990ca1646e)
![1 3](https://github.com/user-attachments/assets/b5c83c4b-2014-4c32-abf7-16ac9f554e6a)
#

2. Change the default username and password to whatever you would like. I changed mine to simply 'admin' and 'password'. 

- Ctrl S and exit the text file.

![2 1](https://github.com/user-attachments/assets/0b23cf1c-1fab-4576-8c4c-facf6c794e51)
![2 2](https://github.com/user-attachments/assets/34783c49-88f6-4c92-8daa-4e311195add7)
#

3. Next we will need to configure the database. Once it asks you to 'enter password', a password has NOT been set up yet, so we can just hit the ENTER key.

- Once you have entered all 3 commands in MariaDB, type in 'exit' and hit enter to exit the MariaDB.

![3 1](https://github.com/user-attachments/assets/f38eab48-b7fd-4691-855a-bc1efd518a35)
![3 2](https://github.com/user-attachments/assets/c908468f-ca9d-4ba7-91cf-25ced00d6c9e)
#

4. Now that we have a database setup, we will need to configure an HTTP web server. 

![4](https://github.com/user-attachments/assets/72cf6a36-b851-48c8-bb26-1b08fd6677e6)
#

5. We will also need to make some configurations on apache2's php file. 
Follow the terminal commands:
 - Select the newest version update. For me, it was version 8.2.
 - Once the php file opens, Ctrl F and search for 'fopen' and make sure both settings are 'ON'. 
 - Ctrl S and exit the php file.

![5 1](https://github.com/user-attachments/assets/7e501a0d-f024-4898-b188-a8f7adea97e1)
#

6. Restart the apache2 webserver.

![6 2](https://github.com/user-attachments/assets/2789a67f-93ec-4a00-85b1-385d6b2ffd52)
#

7. Last step is to go to your web browser and enter '127.0.0.1/DVWA' into the search bar and you should see the DVWA login page. Log in and click the 'restart the web page' button and it is now ready to be used in Kali Linux!

![7 1](https://github.com/user-attachments/assets/eeed0a97-f7b1-4fb7-abb3-eba64c8109c8)
![7 2](https://github.com/user-attachments/assets/72e33e5a-b512-48fd-a74e-8069f1c093cc)


