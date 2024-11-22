## Credential Harvesting with Setoolkit

### Project Overview:
In this project, I will create a spoofed website login page that mimics the hackthissite.org website to simulate credential harvesting, also known as pharming. This attack technique involves redirecting a website's traffic to a fake site and installing a malicious program on the victim's computer to gain access or even mimic a financial institution for monetary gain. I will use tools such as the Social-Engineer Toolkit (Setoolkit) to execute the simulation.

### <ins>Disclaimer</ins>: This project is conducted solely for educational and research purposes within a controlled environment. Unauthorized use of these techniques against real businesses or individuals is illegal and unethical.

#

### Setup and Execution:
To ensure a safe testing environment, I built a home lab using VMware Workstation Pro as my primary virtual machine and installed Kali Linux as the operating system. This setup allows the simulation of attacks in an isolated and secure environment.

#

#### Programs we will be using: 
- VMware Workstation Pro: https://www.broadcom.com/
  - You must create an account
  - Click the drop down menu in the upper right corner and select "VMware Cloud Foundation"
  - Search for VMware Workstation Pro
  - Download for personal use on Windows or Linux
- Kali Linux: https://www.kali.org/get-kali/#kali-virtual-machines
  - For Microsoft Windows: After installing, add the Kali Linux downloaded file as an exclusion in Windows Security > Virus & Threat Protection > Manage Settings > Add or Remove Exclusions > Add Kali Linux.
  - Extract all the files, and it can now be used on VMware as your disk image

#### Vulnerable Website Links:
  - https://www.hackthissite.org/
  - http://testphp.vulnweb.com/login.php 
