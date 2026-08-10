# BLUE
Machine name: Blue | level: Easy | Type: CTF
## INTRODUCTION 
This Machine contains vulnerability the MS17-010 security patch missing. Challenge is to find the users flags in the machine.
## Step 1 : INFORMATION GATHERING
### nmap
nmap -sV -sC -p- 10.48.181.86 --open 
```
Starting Nmap 7.95 ( https://nmap.org ) at 2026-08-10 04:10 EDT
Nmap scan report for 10.48.181.86
Host is up (0.41s latency).
Not shown: 65250 closed tcp ports (reset), 272 filtered tcp ports (no-response)
Some closed ports may be reported as filtered due to --defeat-rst-ratelimit
PORT      STATE SERVICE       VERSION
135/tcp   open  msrpc         Microsoft Windows RPC
139/tcp   open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds  Windows Server 2012 R2 Datacenter 9600 microsoft-ds
3389/tcp  open  ms-wbt-server Microsoft Terminal Service
5985/tcp  open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
47001/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
49152/tcp open  msrpc         Microsoft Windows RPC
49153/tcp open  msrpc         Microsoft Windows RPC
49154/tcp open  msrpc         Microsoft Windows RPC
49155/tcp open  msrpc         Microsoft Windows RPC
49171/tcp open  msrpc         Microsoft Windows RPC
49172/tcp open  msrpc         Microsoft Windows RPC
49199/tcp open  msrpc         Microsoft Windows RPC
Service Info: OSs: Windows, Windows Server 2008 R2 - 2012; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-time: 
|   date: 2026-08-10T08:13:40
|_  start_date: 2026-08-10T08:07:15
| smb-os-discovery: 
|   OS: Windows Server 2012 R2 Datacenter 9600 (Windows Server 2012 R2 Datacenter 6.3)
|   OS CPE: cpe:/o:microsoft:windows_server_2012::-
|   Computer name: WIN-JO6REVNMMMP
|   NetBIOS computer name: WIN-JO6REVNMMMP\x00
|   Workgroup: WORKGROUP\x00
|_  System time: 2026-08-10T01:13:41-07:00
|_nbstat: NetBIOS name: WIN-JO6REVNMMMP, NetBIOS user: <unknown>, NetBIOS MAC: 02:ab:4a:dd:76:f3 (unknown)
| smb-security-mode: 
|   account_used: guest
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: disabled (dangerous, but default)
|_clock-skew: mean: 2h19m59s, deviation: 4h02m30s, median: -1s
| smb2-security-mode: 
|   3:0:2: 
|_    Message signing enabled but not required

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 336.02 seconds
```
## Step 2 : ENUMERATION
### Searching on Web about the services



### Verfying for the vulnerability in Metasploit

## Step3 : EXPLOITATION 
### Metasploit
msfconsole
```
[*] Starting persistent handler(s)...
msf >
```
