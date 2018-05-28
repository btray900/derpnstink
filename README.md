# derpnstink

The goal is to find 4 flags and get some root.


## nmap

![Alt text](./nmap.png?raw=true)


## Browse to site, flag 1

Flag 1 is found looking at the source code and scrolling all the way to the bottom of the page. Also a src to a text file that mentions the hosts file. I'm not sure if it made a difference, I changed it after finding the note. It does mention a username for 'stinky'.

![Alt text](./flag1.png?raw=true)


## dirbuster

weblog dir identifies a Wordpress installation.

![Alt text](./dirbuster.png?raw=true)


## wordpress

admin/admin works to login but not much available.

![Alt text](./admin.png?raw=true)


## wpscan

wpscan identifies a vulnerable plugin which is listed in Metasploit for shell and a couple of users.

![Alt text](./wpscan.png?raw=true)


## low shell


## mysql

crack hashes. wedgie57 for unclestinky

## flag2

Logging in to wordpress as unclestinky shows flag 2 post

![Alt text](./flag2.png?raw=true)


## flag3, user shell

SSH to the vm as stinky with wedgie57 password

## pcap

File mentions pcap, fing another password in the pcap. mrderp user needs a key but su as stinky works fine.

## sudo

sudo shows ALL level for files

## root

create file, run as root

## flag4

cat root flag for victory

## thanks


