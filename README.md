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

<img width="1908" height="1095" alt="Screenshot 2026-01-31 130937" src="https://github.com/user-attachments/assets/edd6ecdc-6e66-4d73-92a3-84b5dd0fc506" />

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

<img width="1910" height="1081" alt="Screenshot 2026-01-31 131024" src="https://github.com/user-attachments/assets/c5dfd52e-4ca2-4791-9a3a-2e977665126b" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="1919" height="1028" alt="Screenshot 2026-01-31 131103" src="https://github.com/user-attachments/assets/2f7065b4-8a62-4bbc-abfb-d5ff7f3c0250" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1913" height="1094" alt="Screenshot 2026-01-31 131144" src="https://github.com/user-attachments/assets/c3b74102-d4d0-48b4-abad-6d53948b2eed" />

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="1919" height="1096" alt="Screenshot 2026-01-31 131239" src="https://github.com/user-attachments/assets/4fadc8b2-13fc-43dd-957f-4714843e10c3" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="1908" height="1073" alt="Screenshot 2026-01-31 131605" src="https://github.com/user-attachments/assets/a679dae0-6667-4f06-ba7d-c6f954ec849e" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

<img width="1920" height="1080" alt="Screenshot_20260131_081450" src="https://github.com/user-attachments/assets/a16f7d0f-1fa5-44b6-8921-af9b5585dcac" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="439" height="693" alt="image" src="https://github.com/user-attachments/assets/e2432d8b-b6a0-46eb-be3e-5cc469d2ca08" />




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


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  <img width="798" height="331" alt="Screenshot_20260131_083307" src="https://github.com/user-attachments/assets/dbe03b52-1e3d-4ad0-b2ae-6ffaf6bf7dd0" />

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

<img width="1300" height="616" alt="image" src="https://github.com/user-attachments/assets/dca595a7-7c45-49af-a400-02bc3c1e51e7" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

