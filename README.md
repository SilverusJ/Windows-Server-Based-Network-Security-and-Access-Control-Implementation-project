# Windows-Server-Based-Network-Security-and-Access-Control-Implementation-project

## Objective

The project aims to establish a secure network environment by configuring three virtual machines, one Windows Server 2012 R2 and two Windows 10 clients while implementing strict access controls and security measures. Key goals include setting up SSL on IIS for secure web access, disabling remote access, enabling firewalls, and hardening the email server with authentication. Additionally, the project aims to enforce password policies, account lockout settings, and controlled software installation for different user roles, ultimately demonstrating effective network security practices

## Skills Learned
  - Network configuration and management
  - Virtual machine setup and administration
  - Implementation of security policies and access controls
  - SSL certificate installation and configuration on IIS
  - VPN setup and management
  - Firewall configuration and management
  - Email server hardening techniques
  - User account management and policy enforcement
  - Troubleshooting software installation issues


## Tools Used
  - Windows Server 2012 R2
  - Windows 10 operating systems
  - Internet Information Services (IIS)
  - VPN software/tools
  - Firewall settings in Windows
  - SMTP Mail Server for email services
  - User account management tools in Windows Server
 

  

## Network Setup

**Virtual Machines**
The project requires setting up three virtual machines:

- One Windows Server 2012 R2 (acting as the main server)

![Screenshot 2024-12-03 221914](https://github.com/user-attachments/assets/b959b596-f8c0-4c29-957a-8b67d95c74cd)  

- Two Windows 10 machines (acting as client machines)

![Screenshot 2024-12-03 231456](https://github.com/user-attachments/assets/f32b6f3e-b484-42d6-8966-fca1199b3a26)



**User Accounts**
The environment includes different user types:
- 4 Sales Users
  
![Screenshot 2024-12-04 014417](https://github.com/user-attachments/assets/6fccdeac-f053-42a4-8d0a-4ed4cfa5b0c4)


![Screenshot 2024-12-04 013259](https://github.com/user-attachments/assets/0c55af14-520a-4699-ac5d-b01bb465cfa6)

  
- 1 Administrator

![Screenshot 2024-12-04 014439](https://github.com/user-attachments/assets/69c9a72a-f838-493b-89f1-0dcc596547c0)
  
- 2 Manager
  
![Screenshot 2024-12-04 014427](https://github.com/user-attachments/assets/26d59925-1ce9-4a0f-aa34-5365921beeff)



## Security Measures

**Web Server Security**

- SSL is configured on Internet Information Services (IIS)

![Screenshot 2024-12-04 020436](https://github.com/user-attachments/assets/570c551b-c9e5-41c9-afc5-08dbe10a1b63)


![Screenshot 2024-12-04 020158](https://github.com/user-attachments/assets/016dbacb-91ba-4290-b1a7-439a68c584d6)

- Client machines can access the website using the IP address 192.168.54.1
  
![Screenshot 2024-12-04 033026](https://github.com/user-attachments/assets/fcf104f8-d766-45af-952b-60ed668c1c89)



  

**Network Security**

- VPN setup is included

![Screenshot 2024-12-04 034720](https://github.com/user-attachments/assets/53187147-39e8-4f71-b5af-21718846988b)


![Screenshot 2024-12-05 230200](https://github.com/user-attachments/assets/607591ac-416c-4c01-ab91-85a76af2a161)


![Screenshot 2024-12-05 231117](https://github.com/user-attachments/assets/119a3a1b-c958-4fe1-9c20-27ce44eea42f)


![Screenshot 2024-12-05 232836](https://github.com/user-attachments/assets/db9f6776-7508-40b6-91da-bc024d59186a)


- Remote Access is disabled on all three machines

![Screenshot 2024-12-05 232901](https://github.com/user-attachments/assets/90905e2a-e4a8-4fd9-a5dd-431f4557b155)


![Screenshot 2024-12-05 235550](https://github.com/user-attachments/assets/3ed37c98-f524-455f-b82f-c591ce626463)

  
- Firewall is enabled on all machines

 ![Screenshot 2024-12-06 001619](https://github.com/user-attachments/assets/70510a28-365a-4519-99a1-01d704287492)


 ![Screenshot 2024-12-06 001631](https://github.com/user-attachments/assets/522fa07a-6825-478a-846f-c20cb7595269)

 

**Email Server Hardening**

- SMTP Mail Server is installed
  
![Screenshot 2024-12-06 005423](https://github.com/user-attachments/assets/a36b6b1a-4f4f-4763-b515-cb7e8663c200)


- Authentication is enabled on the SMTP server
  
![Screenshot 2024-12-06 005813](https://github.com/user-attachments/assets/b700e3cd-49e0-40ce-8942-0a54abaf0015)

Access is restricted to machines using the IP address 127.0.0.1

## Access Control Policies

**Password Policies**

- Minimum password age is set and  Minimum password length is enforced

![Screenshot 2024-12-06 010759](https://github.com/user-attachments/assets/84bee3be-0de4-4a86-ab25-d3a7213a04ff)


**Account Lockout Policies**

- Account lockout duration is configured

![Screenshot 2024-12-06 011513](https://github.com/user-attachments/assets/54800ef1-5714-42a4-a623-1bb69d68a0f9)

  
- Different lockout thresholds are set for:
  
  - Sales computers

![Screenshot 2024-12-06 021338](https://github.com/user-attachments/assets/07c3cf44-b41e-4f31-b15b-6529ba2fcb4c)


  - Manager computers

![Screenshot 2024-12-06 021829](https://github.com/user-attachments/assets/53d0a0d7-db97-4feb-96be-2661aa841583)


  - Server computers

![Screenshot 2024-12-06 021530](https://github.com/user-attachments/assets/470bbbdd-de5f-4f7d-b0e6-e57a7fe06e51)


**Additional Policies**

- All policies are locked

![Screenshot 2024-12-06 022245](https://github.com/user-attachments/assets/92ac3073-96c2-4ef1-b07d-f847a521f492)

  
- Locked-out accounts are managed

![Screenshot 2024-12-06 024141](https://github.com/user-attachments/assets/afed56f0-7ada-4959-870e-75c5327404c6)

  
- Windows Installer is disabled

![Screenshot 2024-12-06 030047](https://github.com/user-attachments/assets/22a6a35b-fa9d-4264-b652-74a6fb159a5f)

  
- Managers are allowed to install software

![Screenshot 2024-12-06 030956](https://github.com/user-attachments/assets/9e64e5a7-4436-4ad2-871d-ec40e13fb20e)


- Legal notices are implemented


![Screenshot 2024-12-06 031930](https://github.com/user-attachments/assets/f8846f73-8b7d-4cb0-b864-5fc0c8cb17fc)


![Screenshot 2024-12-06 033704](https://github.com/user-attachments/assets/eb69b756-1b9c-4e17-91bc-a78f0b26e929)


## Conclusion

This project demonstrates a comprehensive approach to setting up a secure network environment, incorporating various aspects of system administration, network security, and user management.
