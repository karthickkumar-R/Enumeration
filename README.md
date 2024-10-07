# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

## Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## site: 

This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com


![369844097-028acbd9-1cd6-430e-80fa-5ae4032c64b2](https://github.com/user-attachments/assets/3c5cb184-459e-45c3-b254-2e89cb4bb528)


## filetype:
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![369844464-93b1b0ff-6d4d-4713-a743-3698576e04b5](https://github.com/user-attachments/assets/57784564-ce84-48ac-a254-f97f47038b75)

## intext:

This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![369844805-a1a140dc-4a81-4096-a087-047e82264bce](https://github.com/user-attachments/assets/877d7768-f2f1-4c60-a663-83495819383c)

## inurl: 

This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![369845040-91b63f97-4c42-4ab1-b963-c4974e784ffe](https://github.com/user-attachments/assets/c42e9034-aeaf-4272-9780-ad950fbb861b)

## intitle:

This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![369845234-ad903811-29b5-40c0-ae19-38853e9ce871](https://github.com/user-attachments/assets/d6f07261-78f5-44a3-82ef-8323f485201a)

## link:

This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![369845408-46a5588d-c3f5-4090-b3d0-d34e9cce7bd2](https://github.com/user-attachments/assets/1de576b5-65ef-4eb1-bb53-8cba23ca29c3)

## cache: 

This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![369905238-c2ebb68d-50fe-4512-9c1b-07e28c4dde64](https://github.com/user-attachments/assets/958dba4b-4595-45b9-92ec-a03d639f25e3)

 
#DNS Enumeration
##DNS Recon

![369845808-94979a3e-24b5-4ad2-bf1c-ea03ba1301f6](https://github.com/user-attachments/assets/799bd58b-22a1-4363-b0de-d767a7e5caf7)

![369845877-207352be-e5da-42fc-a2b1-0b495642058f](https://github.com/user-attachments/assets/4fc8d859-7447-4279-9c13-6bdbbddbf11d)

## dnsenum

Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

![Screenshot 2024-09-23 154601](https://github.com/user-attachments/assets/f0995c0f-c5ea-42a4-98a2-10e7984f6882)


![Screenshot 2024-09-23 154627](https://github.com/user-attachments/assets/23c1609a-7c86-4fb5-a907-a0dbf8575603)


![Screenshot 2024-09-23 154641](https://github.com/user-attachments/assets/80486bea-f007-456e-8ac6-0fa062a74825)


## smtp-user-enum

Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/user-attachments/assets/c96f155b-0367-431d-b667-07e7745cb4ef)

select any username in the first column of the above file and check the same

![Screenshot 2024-09-23 155751](https://github.com/user-attachments/assets/8503f32f-be87-4e46-b791-76d949beb969)


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
  ![WhatsApp Image 2024-09-25 at 08 34 09_c3bb658e](https://github.com/user-attachments/assets/1f31f3c0-5db5-4f4a-9241-81861bd3696b)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot 2024-09-23 180031](https://github.com/user-attachments/assets/bac7b855-1502-4664-bd70-b9c2cee3d1b8)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully


