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

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

![Screenshot_2024-03-19_23-19-31](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/0843907c-4150-42ce-bfcb-831f9e8a1bd4)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot_2024-03-19_23-20-52](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/acaa3f7b-817d-45f2-83b8-1ac8196cbd45)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot_2024-03-19_23-21-42](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/4a3fc213-5826-470c-82d9-19ae39a1efb1)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![Screenshot_2024-03-19_23-22-42](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/1dd740dd-6304-451e-ae5d-ef6372bc9691)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![Screenshot_2024-03-19_23-25-04](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/8ed81be8-f429-4470-a0dc-c31a7579271e)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot_2024-03-19_23-25-47](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/3194a3a8-0cc8-4ca6-85e5-9915907474c6)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot_2024-03-19_23-26-27](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/6b9dc849-f728-484e-9058-af52537feade)


 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot_2024-03-19_23-29-40](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/79faf031-0aea-43a8-b618-ef6d43913624)

![Screenshot_2024-03-19_23-31-17](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/b707fbb1-77ba-42a2-adab-88ef7b00c527)


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

![Screenshot_2024-03-19_23-32-49](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/a17cae6d-fbff-4da2-8b73-12262deaea09)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


 ![Screenshot_2024-03-19_23-34-42](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/e8af00f5-b355-4aaf-8601-7959aef7840b)

 ![Screenshot_2024-03-19_23-34-42](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/ef6e914d-de63-425b-ae84-83102148db13)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
![Screenshot_2024-03-19_23-41-33](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/34124d32-3ba6-43f0-bd4a-3779fb83ab3a)

 
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot_2024-03-19_23-43-21](https://github.com/Aishwarya-TM/EH-Enumeration/assets/127846109/4fc5b154-7188-4134-95d7-380d778231a3)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

