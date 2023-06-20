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
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/555c3c3e-69e8-445f-ae67-aac374410969)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/7d1967aa-d833-47ba-b1ee-5cc0d5db3b4b)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![3rd](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/3647ba5f-b360-4fd9-b444-7d147b27dba3)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/2c075e04-4246-466e-b6bd-1716ca05b97c)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/0366d7b5-a4af-4378-80a8-32ccda0ec463)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/fa3467d8-8dec-4893-a28a-75f81406dac0)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/ba403934-b2e8-4636-8889-9e55bd04b115)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/93c653e1-abba-49a5-8afe-a144239bb9bf)

![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/52ddadd9-6535-4014-ac64-8c1961624686)

##dnsenum
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
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/4115d76c-a17f-4be3-be2b-96f08177404e)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/9a3a6abc-ea36-4afd-87d2-d8fa052845b6)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/3b1c2b85-9609-41c5-9ca3-3d59cc9979aa)

select any username in the first column of the above file and check the same
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/84c08bb1-a724-4ed2-99e7-67f19fedc3f1)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output

 
  ![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/0b087613-244c-48a8-b3ed-4055120562d8)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/NAVEENMATHIVANAN/Enumeration/assets/119394582/d68a0e81-181e-4b5b-94a0-4658b9c38379)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

