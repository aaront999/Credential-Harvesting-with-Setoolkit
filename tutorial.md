# This is the step-by-step guide and instructions on how to install and configure DVWA in Kali Linux.
    NOTE: If you are looking for the main project content, it is located in the main.md file of this repository.
#
1.  Go to https://github.com/digininja/DVWA and clone the HTTPS code link. Please follow the terminal commands.

![1 1](https://github.com/user-attachments/assets/ef5b0b4c-4e5b-447c-ae3f-d34020e6f684)
#
![Screenshot 2024-11-20 095917](https://github.com/user-attachments/assets/c6a1f6f8-e33f-4851-a957-6082e7c770ba)
![Screenshot 2024-11-20 120037](https://github.com/user-attachments/assets/208384bc-381e-4a79-8f8b-76b01a25df08)
#

2. Change the default username and password to whatever you would like. I changed mine to simply 'admin' and 'password'. 

- Ctrl S and exit the text file.
- Type in 'exit' and hit enter to exit the Maria database.

![Screenshot 2024-11-20 120412](https://github.com/user-attachments/assets/52e03715-c034-4e43-9b0b-5d95efa65895)
![Screenshot 2024-11-20 120443](https://github.com/user-attachments/assets/8f343e61-a609-4e97-8b5d-51d3f781f06e)
#

3. Next we will need to configure the database. Once it asks you to 'enter password', a password has NOT been set up yet, so we can just hit the ENTER key.

![Screenshot 2024-11-20 120636](https://github.com/user-attachments/assets/517513da-7afe-46d1-aaf6-b810fefba76c)
![Screenshot 2024-11-20 121656](https://github.com/user-attachments/assets/be8cc18a-1986-4365-9e72-23f0635abde6)
#

4. Now that we have a database setup, we will need to configure an HTTP web server. 

![Screenshot 2024-11-20 122233](https://github.com/user-attachments/assets/d6bf8aaa-7812-4210-aa11-4abaf89e0190)
#

5. We will also need to make some configurations on a php file. Follow the terminal commands, once the php file opens, Crtl F and search for 'fopen' and make sure both settings are ON. Crtl S and exit the php file.

![Screenshot 2024-11-20 122546](https://github.com/user-attachments/assets/9cd913e7-eac3-4418-bb1e-481763005749)
#

6. Restart the apache2 webserver.

![Screenshot 2024-11-20 122718](https://github.com/user-attachments/assets/2e400de6-3fc4-479b-b98b-84898e4e9afb)
#

7. Last step is to go to your web browser and enter '127.0.0.1/DVWA' into the search bar and you should see the DVWA login page. Log in and click the 'restart the web page' button and it is now ready to be used in Kali Linux!

![Screenshot 2024-11-20 122741](https://github.com/user-attachments/assets/443b344f-39cb-4c3a-ae4e-6634cf5480b0)
![Screenshot 2024-11-20 122833](https://github.com/user-attachments/assets/e7f0a440-7562-40e6-abfc-f0d394ace58f)





   
