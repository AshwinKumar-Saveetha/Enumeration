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

| Operator    | Description                        | Example Usage           |
| ----------- | ---------------------------------- | ----------------------- |
| `site:`     | Search within a specific domain    | `site:example.com`      |
| `inurl:`    | Search in URL                      | `inurl:admin`           |
| `intitle:`  | Search in page title               | `intitle:"index of"`    |
| `filetype:` | Search by file type                | `filetype:pdf`          |
| `intext:`   | Search inside page text            | `intext:"confidential"` |
| `link:`     | Pages that link to a specific site | `link:example.com`      |
| `cache:`    | View cached version of a site      | `cache:example.com`     |
| `ext:`      | Same as filetype                   | `ext:xls`               |

 ## Architecture 
 ```
+----------------------+
|   Attacker / Hacker  |
|   (Browser & Google) |
+----------+-----------+
           |
           | Google Dork Queries
           v
+---------------------------+
|       Google Search       |
+---------------------------+
           |
           | Indexed Public Content
           v
+---------------------------+
|   Target Websites / Data  |
| - Leaked files            |
| - Open directories        |
| - Sensitive info          |
+---------------------------+

```

# Output:
# SITE:

<img width="873" height="907" alt="image" src="https://github.com/user-attachments/assets/3be38a15-05d5-4163-bd5b-b3386d533c1b" />


# INURL

<img width="1322" height="1020" alt="Screenshot 2025-09-04 084333" src="https://github.com/user-attachments/assets/e1639af9-74d3-46ae-ba03-f4069e62388d" />

# INTITLE

<img width="1331" height="725" alt="Screenshot 2025-09-04 084620" src="https://github.com/user-attachments/assets/8e1c5da3-76c0-4a74-a38a-d50540def9c0" />

# FILETYPE

<img width="1317" height="1004" alt="Screenshot 2025-09-04 084754" src="https://github.com/user-attachments/assets/2303f865-778a-409d-b9b1-f50c9b5695dc" />

# INTEXT

<img width="1323" height="997" alt="Screenshot 2025-09-04 084837" src="https://github.com/user-attachments/assets/6fbad445-10d7-475e-9ae5-47f69a71395a" />

# LINK

<img width="1327" height="1008" alt="Screenshot 2025-09-04 084940" src="https://github.com/user-attachments/assets/e51fb09d-f0d7-4333-8523-696ace8e7212" />

# EXT

<img width="1318" height="1016" alt="image" src="https://github.com/user-attachments/assets/b18edf71-d94e-4958-b46b-4b351eba3a43" />

# DNS Enumeration

<img width="663" height="667" alt="image" src="https://github.com/user-attachments/assets/bb72e509-00f0-4815-9577-d70be7bac04a" />
<br>
<img width="782" height="537" alt="image" src="https://github.com/user-attachments/assets/d5d6889d-fe3d-4b2f-8980-d5e27ba7ad3b" />

## DNS Recon

<img width="1065" height="781" alt="image" src="https://github.com/user-attachments/assets/f918dc34-f35c-490f-aa28-ffa01a88270b" />
<br>


| Record Type | Meaning                        | Example Output                   |
| ----------- | ------------------------------ | -------------------------------- |
| A           | Host to IPv4 address           | `example.com -> 93.184.216.34`   |
| AAAA        | Host to IPv6 address           | `example.com -> ::1`             |
| MX          | Mail server info               | `mail.example.com`               |
| NS          | Name servers                   | `ns1.example.com`                |
| TXT         | Misc data (SPF, verifications) | `v=spf1 include:_spf.google.com` |
| CNAME       | Canonical names (aliases)      | `www -> example.com`             |

## Common Tools Used (Kali Linux)

| Tool           | Description                                | Usage Example                           |
| -------------- | ------------------------------------------ | --------------------------------------- |
| `nslookup`     | DNS lookup tool (simple queries)           | `nslookup example.com`                  |
| `dig`          | DNS lookup utility (detailed)              | `dig example.com any`                   |
| `host`         | Simple DNS querying tool                   | `host example.com`                      |
| `dnsenum`      | Perl script to enumerate DNS info          | `dnsenum example.com`                   |
| `fierce`       | DNS scanner to locate non-contiguous IPs   | `fierce -dns example.com`               |
| `dnsrecon`     | Powerful DNS enumeration script            | `dnsrecon -d example.com -a`            |
| `theHarvester` | Subdomain enumeration using search engines | `theHarvester -d example.com -b google` |


## OUTPUT:
# NSLOOKUP

<img width="272" height="192" alt="Screenshot 2025-09-08 093225" src="https://github.com/user-attachments/assets/ab1f3344-babd-4ae3-91b0-36cabb8debae" />

# DIG

<img width="1014" height="643" alt="Screenshot 2025-09-08 093144" src="https://github.com/user-attachments/assets/9a236c01-3088-42db-87c9-d17a7a80d725" />

# HOST

<img width="509" height="210" alt="Screenshot 2025-09-08 093515" src="https://github.com/user-attachments/assets/a9b10b7d-77a5-47c2-8da7-86cfade42f92" />

# DNSENUM

<img width="664" height="667" alt="Screenshot 2025-09-08 091351" src="https://github.com/user-attachments/assets/50852a95-da93-4e7c-a196-1e4402382fbe" />
<br>
<img width="782" height="538" alt="Screenshot 2025-09-08 091422" src="https://github.com/user-attachments/assets/b2e9ee0d-d036-4f36-abe2-cf1a7de51e43" />

# DNSRECON

<img width="1065" height="781" alt="Screenshot 2025-09-08 092305" src="https://github.com/user-attachments/assets/de666dc4-4624-4069-b8cf-71ee9bc40632" />
<br>
<img width="1056" height="656" alt="Screenshot 2025-09-08 092350" src="https://github.com/user-attachments/assets/fb4837d3-7991-48e9-8e53-3baaa026c3a9" />


# FIERCE
<img width="763" height="996" alt="fierce exp 3" src="https://github.com/user-attachments/assets/683ca218-93f0-49d8-9bfa-169d06cf2226" />

# HARVESTER
<img width="723" height="725" alt="Harvester exp 3" src="https://github.com/user-attachments/assets/be204124-6c7b-4dc7-a434-4d6c71cbccf9" />

## Architecture Diagram 
```
+-------------------+        +------------------+       +------------------+
|                   |        |                  |       |                  |
|   Attacker (You)  +------->|   Target Server   +<----->+    DNS Server    |
| Kali Linux / Parrot|       | (Mail / DNS Host) |       |  (Authoritative) |
+---------+---------+        +---------+--------+       +---------+--------+
          |                            ^                          ^
          |                            |                          |
          |                            |                          |
          |           +-----------------------------+            |
          |           |      Information Tools      |            |
          |           |-----------------------------|            |
          |           | smtp-user-enum              |            |
          |           | nmap --script smtp-enum-*   |            |
          |           | dnsenum                     |<-----------+
          |           +-----------------------------+
          |
          v
+-----------------------------+
|   Output/Report             |
|  - Usernames Found          |
|  - MX Records / Zones       |
|  - Subdomains / IPs         |
+-----------------------------+

```

## dnsenum
**Purpose:** A multithreaded Perl script to enumerate information from DNS servers.

**Use case:** Performs DNS zone transfers, brute force subdomains, and gather host IPs.

```
dnsenum example.com
```

## Output:
<img width="658" height="471" alt="Screenshot 2025-08-25 204202" src="https://github.com/user-attachments/assets/7b5ee759-3c92-4ec1-a3fc-7e52ccb99aa4" />




## smtp-user-enum
**Purpose:** Standalone tool used to enumerate valid users by using the VRFY, EXPN, or RCPT TO commands.

**Use case:** Brute-forces SMTP to find users.

```
smtp-user-enum -M VRFY -U users.txt -t <target-ip>
```
  
 ## Output
<img width="680" height="370" alt="Screenshot 2025-08-25 202131" src="https://github.com/user-attachments/assets/e4c7471f-0524-4c3c-85f0-80ef250ebb1b" />



## nmap –script smtp-enum-users.nse <hostname>

**Purpose:** Uses smtp-enum-users NSE script to enumerate valid users on an SMTP server.

**Use case:** Helps identify email accounts on mail servers.

```
nmap -p 25 --script smtp-enum-users.nse <target-ip>
```
## OUTPUT:
<img width="681" height="137" alt="Screenshot 2025-08-25 202159" src="https://github.com/user-attachments/assets/bc1327b9-914d-47f7-b4df-c5c81c96d293" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
