1. I begin by opening the linux terminal and entering the command 'sudo setoolkit' to launch the program.

![1 1](https://github.com/user-attachments/assets/8693f5f9-f669-4bf1-b70c-f4a52578a506)
#

2. Once Setoolkit is launched, I navigate to Social-Engineering Attacks > Website Attack Vectors > Credential Harvester Attack Method > Site Cloner to begin cloning the login page of my target website.  

![1 2](https://github.com/user-attachments/assets/f9108a95-a473-4ea9-9e70-169170688fcb)
![1 3](https://github.com/user-attachments/assets/97be5489-cbd8-4f1c-b133-7a4b15554537)
#

3. Next, I copied the URL of the website I intend to fabricate as legitimate, in this case: hackthissite.org, in order to create a convincing replica for the credential harvesting attack.

![2 01](https://github.com/user-attachments/assets/af80ab93-4830-4645-afea-6c3c6fca0ae5)
#

4. Then, I entered the IP address or domain name of the server where the spoofed website will be hosted, which, in my case, is the Kali Virtual Machine's IP address: 128.0.0.1. 
- After that, we need to paste the URL of the legitimate website in the command to initiate the cloning process.

![2 1](https://github.com/user-attachments/assets/02b2e694-97cd-43f3-849d-554c26097221)
#

5. After the cloning process is complete, I open a new browser tab and enter the spoofed website's domain name/ip, '128.0.0.1' in the search bar. 
 - The cloned website is now ready to be used as a credential harvester.  
 - Which we can now test the webpage by inputting fake credentials and successfully capture the expected data, verifying the effectiveness of the attack. 
 - In a real attack scenario, the attacker would now have access to the victim’s credentials, allowing them to log in and potentially perform malicious activities without the victim ever even realizing it!
 
![3 1](https://github.com/user-attachments/assets/7c00c6b7-16d1-47c0-a4a8-5ba317810c8c)
![3 2](https://github.com/user-attachments/assets/680f4de5-c3b6-4afd-a909-92e88db302ea)
#

6. I tested this method on another intentionally vulnerable website and successfully received the expected output as well. Notice that both cloned webpages look identical to their legitimate counterpart, making it highly convincing to an unsuspecting user. When combined with a phishing email campaign, this attack technique can be an effective way to socially engineer a victim.

![4 01](https://github.com/user-attachments/assets/17313ac1-2734-4057-a676-4d2f9e20cf9a)
![4 02](https://github.com/user-attachments/assets/191325ef-23fb-4013-ae57-d13aefb86dd4)
#
![5 1](https://github.com/user-attachments/assets/f6371a6c-68bb-4bda-88c8-9ffabac701a4)
![5 2](https://github.com/user-attachments/assets/f4bd8ea8-28e1-4654-b4af-af1bbaea39a7)
#
