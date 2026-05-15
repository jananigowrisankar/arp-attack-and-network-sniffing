# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks

# AIM:

To explore network sniffing and ARP Attacks

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## ARP Attacks:  
ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 
Boot kali and Windows7 virtual machines.
In windows 7 give the command arp -a
## OUTPUT:

<img width="1121" height="795" alt="image" src="https://github.com/user-attachments/assets/a16b5e45-ae6d-4edf-a3c2-902711dcea0f" />

It is used to displays the ARP table/cache of your machine.

From kali linux issue the command :
sudo arpspoof -i eth0 -t <target system> <gateway>

The command uses `sudo` to execute with administrator privileges, which are necessary for network packet manipulation. `arpspoof` is a network security tool that sends forged ARP (Address Resolution Protocol) messages on a local network and is commonly used in authorized cybersecurity labs to demonstrate ARP spoofing and man-in-the-middle attack concepts. The option `-i eth0` specifies the network interface (`eth0`) through which the packets are sent, while `-t <target_ip>` identifies the victim system’s IP address. The `<gateway_ip>` refers to the router or default gateway address, and the command tricks the target machine into believing that the attacker’s MAC address belongs to the gateway, causing network traffic to pass through the attacker’s system. Humanity really built networks on “trust me bro” architecture and acted surprised later.

## OUTPUT:

 dsniff:

<img width="1157" height="310" alt="image" src="https://github.com/user-attachments/assets/cec31fb3-08d8-4966-8520-8dbcd3c4c919" />

`dsniff` is a network packet sniffing tool used to capture and analyze traffic within a local network, mainly in authorized cybersecurity and ethical hacking labs. Its primary purpose is to monitor packets travelling across the network and identify data transmitted through insecure, unencrypted protocols such as HTTP, FTP, Telnet, POP3, and IMAP. Since these protocols may send information in plain text, the tool can sometimes display sensitive data like usernames and passwords if proper encryption is not used. A stunning example of early internet design where people collectively decided privacy was apparently optional.


In Metasploit open the ftp console as below. Also you can try other ftp websites ftp.vim.org
## OUTPUT:

<img width="898" height="445" alt="image" src="https://github.com/user-attachments/assets/c0f58de7-c56d-43ed-93f7-416a1d3f0b12" />



In Kali issue the following commands:
sudo dsnifff
## OUTPUT:

<img width="832" height="155" alt="image" src="https://github.com/user-attachments/assets/ffc2bc8d-979d-4017-8638-7aafa2d6de8d" />


`dsniff` is a network packet sniffing tool used to capture and analyze traffic within a local network, mainly in authorized cybersecurity and ethical hacking labs. Its primary purpose is to monitor packets travelling across the network and identify data transmitted through insecure, unencrypted protocols such as HTTP, FTP, Telnet, POP3, and IMAP. Since these protocols may send information in plain text, the tool can sometimes display sensitive data like usernames and passwords if proper encryption is not used. A stunning example of early internet design where people collectively decided privacy was apparently optional.
 
Invoke the wireshark and examine the various menus  and controls of the tool:

<img width="947" height="936" alt="image" src="https://github.com/user-attachments/assets/e3739dd1-a134-4025-a125-e1a344793b6e" />


## ARP POISONING:

<img width="957" height="1088" alt="image" src="https://github.com/user-attachments/assets/b2112209-c0b8-4f7f-ba0a-da05b8d98b31" />

<img width="957" height="1092" alt="image" src="https://github.com/user-attachments/assets/874c09ac-a4e5-4e20-a8a3-6336f2fa3332" />

<img width="953" height="118" alt="image" src="https://github.com/user-attachments/assets/17dfb778-70c5-4c87-b149-a5ebc5884e27" />

<img width="955" height="122" alt="image" src="https://github.com/user-attachments/assets/668eceec-f194-4f36-bf1e-e7ba1d69b8aa" />

<img width="1578" height="786" alt="image" src="https://github.com/user-attachments/assets/13936af4-0e5c-4393-9ab7-08911ad1fe26" />


## RESULT:
The kali linux tools for ARP Attack and Network Sniffing were identified successfully
