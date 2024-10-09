# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system

## OUTPUT:

![image](https://github.com/user-attachments/assets/c824ef58-04c9-4a62-b660-e5d7b1afc7e9)

## Invoke msfconsole
## OUTPUT:

![image](https://github.com/user-attachments/assets/ae380cac-cee0-46da-adac-e257c795eebf)

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

![image](https://github.com/user-attachments/assets/af1a1a1b-0f1b-4821-96fa-c64639b06379)

## Port scanning:
## msf > nmap -sT 192.168.1810/24-p1-1000

![image](https://github.com/user-attachments/assets/a102d2db-8b94-445c-a774-fe3001bd5543)

## msf > db_nmap 192.168.181.0/24

![image](https://github.com/user-attachments/assets/5d52ae35-cf10-4690-b10a-b21fe80ef3cd)

## kali > ls-l

![image](https://github.com/user-attachments/assets/5b435f09-b3cd-4b3e-a4e5-50063d340c01)

## search

![image](https://github.com/user-attachments/assets/37255d82-f21c-494b-abe8-d998c2629236)

## MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port. db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

![image](https://github.com/user-attachments/assets/a7c92753-851d-4a5d-80d3-cd789618582e)

## db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

![image](https://github.com/user-attachments/assets/067276dd-8811-4c07-aa95-4eb8e8f08126)

## search

![image](https://github.com/user-attachments/assets/aee819de-6f1b-49bd-a42d-b67ae9e2e225)

## use 11 Or: use auxiliary/scanner/mysql/mysql_version

![image](https://github.com/user-attachments/assets/42420fca-1ecd-4b3a-822e-a0cbed7e6b8d)

## Use the set rhosts command to set the parameter and run the module, as follows:

![image](https://github.com/user-attachments/assets/f91b4316-903d-45e8-bab2-714ea4968bf9)

## After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module.

![image](https://github.com/user-attachments/assets/a5bc7ec2-30c8-4dd0-a8f0-82f0017dc569)

## /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt

![image](https://github.com/user-attachments/assets/6b1d0d80-3d71-4986-8806-b6b0e3454452)

![image](https://github.com/user-attachments/assets/de4f43e7-fded-484a-ab4a-c1a1727ce435)


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
