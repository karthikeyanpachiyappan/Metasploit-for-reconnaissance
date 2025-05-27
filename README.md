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
![image](https://github.com/user-attachments/assets/331b02d5-6e10-4166-8df4-05182ad7a0c2)
Invoke msfconsole:
## OUTPUT:
![image](https://github.com/user-attachments/assets/4d9a015a-07c3-47ff-b1b2-d2ed86fc87c9)
Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

## OUTPUT:
![image](https://github.com/user-attachments/assets/0192b421-ef55-4a31-932e-ee7b07c2b502)
![image](https://github.com/user-attachments/assets/c455522a-c6a7-40f1-ae81-77a52559cc4a)
![image](https://github.com/user-attachments/assets/9c45c5aa-0aa9-4e18-ad56-34b7ecd313d4)
![image](https://github.com/user-attachments/assets/79987339-84ef-4ad0-90e1-f3dcb83c5ff1)
![image](https://github.com/user-attachments/assets/67f04375-954f-4935-9965-b3bc111e52e0)


Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).
msf >  nmap -sT 192.168.228.34/24 -p1-1000
## OUTPUT:

![image](https://github.com/user-attachments/assets/1b474d4d-52a3-4d62-8efc-678c2d54ad18)


use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.
msf > db_nmap 192.168.228.34/24
## OUTPUT:
![image](https://github.com/user-attachments/assets/12668bd5-a3c3-4744-bce2-8f17c56dacf3)


![image](https://github.com/user-attachments/assets/cced965a-29df-4e9c-b1b1-53c20c4f249c)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules.
cd /usr/share /metasploit-framework/modules/auxiliary
kali > ls -l
## OUTPUT:

![image](https://github.com/user-attachments/assets/0b28240b-00bf-4b14-82ab-afb6e858ae06)


Search is a powerful command in Metasploit that you can use to find what you want to locate. 
msf >search name:Microsoft type:exploit
## OUTPUT:
![image](https://github.com/user-attachments/assets/b04f859e-7029-4b42-a6aa-aad212c41371)


The info command provides information regarding a module or platform,
## OUTPUT:
![image](https://github.com/user-attachments/assets/9c3de984-4932-4663-97cc-46d7bea66262)


##MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port.
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
## OUTPUT:
![image](https://github.com/user-attachments/assets/a6f9a49e-e5b7-49a6-8a61-f8a5ad65c878)

![image](https://github.com/user-attachments/assets/48f2459e-43a0-4774-9815-1ce32fea5ad1)

![image](https://github.com/user-attachments/assets/98caec0a-7eec-4499-aed4-2abc5abb461d)

![image](https://github.com/user-attachments/assets/44a64102-d4bb-454a-a716-ae1b99bd5b36)


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
