# Jarkom-Modul-1-I07-2022

Group Members:
1. Denta Bramasta Hidayat (5025201116)
2. Ghazi
3. Rivaldo


## Question 1
>Mention the website server used on “monta.if.its.ac.id”? 

answer: `http.host contains monta.if.its.ac.id`

[ss]

## Question 2
>Ishaq was confused looking for TA topics for this semester, then he came to the monta website and found the topic details on the website “monta.if.its.ac.id”, what TA title did Ishaq open?

answer: `ip.host == 103.94.189.5 && tcp contains detailTopik`

[ss]

## Question 3
>Filter so that wireshark only shows packets going to port 80!

answer: `display filter tcp.dstport == 80 || udp.port == 80`

[ss]

## Question 4
>Filter so that wireshark only picks up packets coming from port 21!

answer: `tcp.srcport == 21 || udp.srcport == 21`

[ss]

## Question 5
>Filter so that wireshark only picks up packets coming from port 443!

answer: `tcp.srcport == 443 || udp.srcport == 443`

[ss]

## Question 6
>Filter so that wireshark only shows packets going to lipi.go.id !

answer: `tcp contains lipi.go.id`

[ss]

## Question 7
>Filter so that wireshark only picks up packets coming from your ip! Find your ip in cmd with ipconfig

answer: `host 192.168.137.1`

[ss]

## Question 8
>Browse the flow of packets in the given .pcap file, look for useful information in the form of a conversation between two students regarding cheating in practicum activities. The conversation is reported to use a network protocol with a high level of reliability in its data exchange so you need to apply a filter with that protocol.

answer: `tcp.flags.syn == 1 && tcp.flags.ack ==1`

## Question 9
>There are reports of file exchanges made by the two students in the conversations obtained, look for the file in question! To facilitate reporting to superiors, name the file found in the format [group_name].des3 and save the output file with the name “flag.txt”

answer: `tcp.port == 9002 || udp.port == 9002` and for decrypt des3 using command `Openssl des3 -d -in I07.des3 -out flag.txt` with password `nakano`

[ss]

## Question 10
>Find the secret password (flag) of the above-mentioned underground organization!
password: `nakano` and for decrypt des3 using command `Openssl des3 -d -in I07.des3 -out flag.txt`

[ss]


### Trouble 
In macOS for number 9 and 10 we cannot decrypt using des3 I dont know why. the output always shown as `bad decrypt` 


