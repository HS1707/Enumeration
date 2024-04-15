# Enumeration Techniques
# Explore Google hacking and enumeration 

## AIM:
To use Google for gathering information and perform enumeration of targets

## PROCEDURE:

1. Install kali linux either in partition or virtual box or in live mode
2. Investigate on the various Google hacking keywords and enumeration tools as follows:
3. Open terminal and try execute some kali linux commands
4. 
## Pen Test Tools Categories:  
Following Categories of pen test tools are identified:
Information Gathering.
Google Hacking:
Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.

Following searches for all the sites that is in the domain yahoo.com

![Screenshot (86)](https://github.com/gpavithra673/Enumeration/assets/93427264/0a7b053a-6498-497f-a797-613c4bb683e1)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot (85)](https://github.com/gpavithra673/Enumeration/assets/93427264/51a75fb3-7b2f-4694-ae8a-6fda17a0ae66)


 intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![Screenshot (84)](https://github.com/gpavithra673/Enumeration/assets/93427264/85604250-db13-4dc1-91cb-56fb0bd4f4a9)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![Screenshot (83)](https://github.com/gpavithra673/Enumeration/assets/93427264/2bd89928-3f3f-4cc4-9017-9713825dc75b)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot (82)](https://github.com/gpavithra673/Enumeration/assets/93427264/7a9fc92a-faae-4650-b89c-b62ea5dcb9c1)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![Screenshot (81)](https://github.com/gpavithra673/Enumeration/assets/93427264/e0a40d16-e3b1-41b6-b3b9-752f8ffd904b)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![Screenshot (80)](https://github.com/gpavithra673/Enumeration/assets/93427264/c4173f65-5404-4dab-95d4-627da578fe20)

## DNS Enumeration

## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:
![Screenshot (75)](https://github.com/gpavithra673/Enumeration/assets/93427264/9c0158d4-eab4-4ccd-bcdb-92d382e4aa0f)
![image](https://github.com/gpavithra673/Enumeration/assets/93427264/a7dd190f-61ce-4e0d-97aa-f81d3c6170c6)

## Dnsenum
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

### Output:
![image](https://github.com/gpavithra673/Enumeration/assets/93427264/5db80a37-fb83-4cf9-b3a4-44f473ebc9e5)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
## Output:
![image](https://github.com/gpavithra673/Enumeration/assets/93427264/1d25a1e3-d4d0-4d23-b0f0-45be40a37add)


## Telnet for smtp enumeration: 
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/gpavithra673/Enumeration/assets/93427264/4be1c254-8a5d-435c-a5b3-a9769b1e43c6)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully.
