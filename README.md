## Credential Harvesting with Setoolkit

### Project Overview:
In this project, I will create a spoofed website login page mimicking the Damn Vulnerable Web Application (DVWA) to simulate credential harvesting on a victim's host using the Social-Engineer Toolkit (Setoolkit).

### <ins>Disclaimer</ins>: This project is conducted solely for educational and research purposes within a controlled environment. Unauthorized use of these techniques against real websites or individuals is illegal and unethical.

#

### Setup and Execution:
To ensure a safe testing environment, I built a home lab using VMware Workstation Pro as my primary virtual machine and installed Kali Linux as the operating system. This setup allows the simulation of attacks in an isolated and secure environment.
  - The Damn Vulnerable Web Application (DVWA) was installed and configured on Kali Linux to serve as the target application for testing.
  - I will include a step-by-step guide and instructions on how to install and configure DVWA in Kali Linux, which will be documented in the <em>**tutorial.md**</em> file.
  - The main project details, including the process and findings, will be documented in the <em>**main.md**</em> file.

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
- Damn Vulnerable Web Application (DVWA): https://github.com/digininja/DVWA
