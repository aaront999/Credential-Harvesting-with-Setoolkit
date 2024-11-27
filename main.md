# Part 1: Understanding Setoolkit’s Credential Harvester

1. I started by opening the linux terminal and ran the command 'sudo setoolkit' to launch the Social Engineering Toolkit (SET).

![1 1](https://github.com/user-attachments/assets/8693f5f9-f669-4bf1-b70c-f4a52578a506)
#

2. Once Setoolkit is launched and running, I navigate to the appropriate sections: Social-Engineering Attacks > Website Attack Vectors > Credential Harvester Attack Method > Site Cloner to set up the cloning process of the login page of my target website.  

![1 2](https://github.com/user-attachments/assets/f9108a95-a473-4ea9-9e70-169170688fcb)
![1 3](https://github.com/user-attachments/assets/97be5489-cbd8-4f1c-b133-7a4b15554537)
#

3. I chose hackthissite.org as my target site, intending to replicate it as part of my test environment. I copied the target URL for cloning.

![2 01](https://github.com/user-attachments/assets/af80ab93-4830-4645-afea-6c3c6fca0ae5)
#

4. Next, I entered the IP address or domain name of the server where the spoofed website will be hosted, which, in my case, is the Kali VM's IP address: 128.0.0.1. After that, I paste the URL of the legitimate website in the command to initiate the cloning process.

![2 1](https://github.com/user-attachments/assets/02b2e694-97cd-43f3-849d-554c26097221)
#

5. After cloning, I tested my setup by opening a browser and navigated to 128.0.0.1, the spoofed website's web address. I simulated user interactions by entering fake credentials, which were successfully captured on my terminal end.
 - In a real attack scenario, the attacker would now have access to the victim’s credentials, allowing them to log in and potentially perform malicious activities without the victim ever even realizing it!
 
![3 1](https://github.com/user-attachments/assets/7c00c6b7-16d1-47c0-a4a8-5ba317810c8c)
![3 2](https://github.com/user-attachments/assets/680f4de5-c3b6-4afd-a909-92e88db302ea)
#

6. To ensure reliability, I tested this method on another intentionally vulnerable site and successfully received the expected output as well. Notice that both cloned webpages look identical to their legitimate counterpart, making it highly convincing to an unsuspecting user. When combined with a phishing email campaign, this attack technique can be an effective way to socially engineer a victim.

![4 01](https://github.com/user-attachments/assets/17313ac1-2734-4057-a676-4d2f9e20cf9a)
![4 02](https://github.com/user-attachments/assets/191325ef-23fb-4013-ae57-d13aefb86dd4)
![5 1](https://github.com/user-attachments/assets/f6371a6c-68bb-4bda-88c8-9ffabac701a4)
![5 2](https://github.com/user-attachments/assets/f4bd8ea8-28e1-4654-b4af-af1bbaea39a7)
#

# Part 2: Simulating a Credential Harvesting Attack
 
#### Now that I have validated the reliability of this tool, I wanted to explore its application in a controlled, ethical scenario to simulate an attack flow for educational purposes. My goal was to better understand how attackers might retrieve credentials, allowing me to develop stronger countermeasures and security awareness strategies for protecting users against such threats.
#

7. First I began by crafting a fake Google Support email.

![1 1](https://github.com/user-attachments/assets/dd8a6ce5-1748-44ae-b28f-246654781a24)
![1 2](https://github.com/user-attachments/assets/e19131b3-eff2-4953-acc0-de2e637f5c20)
![1 3](https://github.com/user-attachments/assets/98fc8272-68ef-46d9-808f-e7b6fb6835cb)
#

8. Once I have my fake Google Support email set up, I created a phishing email to closely resemble something Google might send to any user. 
- There are no links for the victim to click into yet, but I will be making that next. 

![2 1](https://github.com/user-attachments/assets/8b26aae8-9222-45da-b31b-256b43d9c149)
#

9. I then went to dns.checker.org to convert my attack box's ip address into decimal form to make our malicious link look more legitimate to an unsuspecting user. 

![3 1](https://github.com/user-attachments/assets/1f5b0752-1d19-4cb9-a228-130ab7cf6979)
#

10. Now our malicious domain is ready to be used: hxxp[://]google[.]com@2147483649. 
- By putting the @ symbol instead of a slash, when searched in a browser, it will ignore everything before the @ symbol and will re-direct the victim to my spoofed website's login page. 

![3 2](https://github.com/user-attachments/assets/50369e9a-a248-479e-aba5-d5765b4a2be0)
#

11. I edited the hyperlinks of my fake Google Support email and 'Google Support login page' to my spoofed website's address so that in the event that a victim is fooled into thinking this email is legitimate, they would be redirected to the spoofed site and any activity that happens will be logged and received on my attack box's terminal. 

![4 1](https://github.com/user-attachments/assets/3f9dff36-1ca6-43b0-89dd-77460112f44c)
![4 2](https://github.com/user-attachments/assets/2772ae7e-ee12-4bdb-9a98-6650c9ddffdf)
#

12. Once I set up the required configurations in Setoolkit and the tool is actively listening for input, my phishing email is prepared and ready to be sent.

![5 2](https://github.com/user-attachments/assets/8cee8439-ec9d-4957-81f8-32e3ed549072)
![4 3](https://github.com/user-attachments/assets/251cc5e4-dd44-43ee-992e-ee3dbc5aab8d)
#

13. If the victim falls for this phishing attack and clicks on one of the malicious links, they are redirected to my spoofed website. Upon entering their credentials, the attack is successful, and their activity and information is captured.

![6 1](https://github.com/user-attachments/assets/564a7076-5199-437f-bc98-20ebdb8570e9)
![6 2](https://github.com/user-attachments/assets/e5c6b8bb-735f-4526-a6ba-cb12e9c2dbff)
#
