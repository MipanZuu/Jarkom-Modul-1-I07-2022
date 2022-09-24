# Jarkom-Modul-1-I07-2022

Group Members:
1. Denta Bramasta Hidayat (5025201116)
2. Ghazi Buana Dewa (5025201074)
3. Rivaldo Panangian Tambunan (5025201134)


## Question 1
>Mention the website server used on “monta.if.its.ac.id”? 

answer: `http.host contains monta.if.its.ac.id`

![unnamed](https://user-images.githubusercontent.com/101728396/192084678-f16fae95-c3f9-4bef-bf5a-85d9fc31e5b6.png)

Nginx display/tcp.stream

![ss1](https://user-images.githubusercontent.com/101728396/192085073-6475bed7-85d8-4bec-82cd-ee1000fc2d50.jpg)

## Question 2
>Ishaq was confused looking for TA topics for this semester, then he came to the monta website and found the topic details on the website “monta.if.its.ac.id”, what TA title did Ishaq open?

answer: `ip.host == 103.94.189.5 && tcp contains detailTopik`

![ss2](https://user-images.githubusercontent.com/101728396/192085145-29f97b3a-aebc-4624-84da-cc8c99853154.gif)

## Question 3
>Filter so that wireshark only shows packets going to port 80!

answer: `display filter tcp.dstport == 80 || udp.port == 80`

![ss3](https://user-images.githubusercontent.com/101728396/192085190-21ca764f-5e56-49f3-b6a4-bc2fc8f825f4.jpg)

## Question 4
>Filter so that wireshark only picks up packets coming from port 21!

answer: `tcp.srcport == 21 || udp.srcport == 21`

![ss4](https://user-images.githubusercontent.com/101728396/192085278-bebf1488-4156-4692-9476-49ff1dc99246.jpg)

## Question 5
>Filter so that wireshark only picks up packets coming from port 443!

answer: `tcp.srcport == 443 || udp.srcport == 443`

![ss5](https://user-images.githubusercontent.com/101728396/192085319-63b925ea-80ca-401e-847f-1e1bbb8561fd.jpg)

## Question 6
>Filter so that wireshark only shows packets going to lipi.go.id !

answer: `tcp contains lipi.go.id`

![ss6](https://user-images.githubusercontent.com/101728396/192085371-f2983aad-fce9-43a5-8501-15b4d35a3a50.jpg)

## Question 7
>Filter so that wireshark only picks up packets coming from your ip! Find your ip in cmd with ipconfig

answer: `host 192.168.137.1`

![ss7](https://user-images.githubusercontent.com/101728396/192085405-cb49963a-7c14-48da-a2f0-292becb993db.jpg)

## Question 8
>Browse the flow of packets in the given .pcap file, look for useful information in the form of a conversation between two students regarding cheating in practicum activities. The conversation is reported to use a network protocol with a high level of reliability in its data exchange so you need to apply a filter with that protocol.

answer: `tcp.flags.syn == 1 && tcp.flags.ack ==1`

![ss8](https://user-images.githubusercontent.com/101728396/192085625-f29ba1c2-53b5-410d-84bd-2be440e7364a.jpg)

![ss9](https://user-images.githubusercontent.com/101728396/192085580-58ec6141-1238-410d-981e-20c9c618c31a.jpg)

## Question 9
>There are reports of file exchanges made by the two students in the conversations obtained, look for the file in question! To facilitate reporting to superiors, name the file found in the format [group_name].des3 and save the output file with the name “flag.txt”

answer: `tcp.port == 9002 || udp.port == 9002` and for decrypt des3 using command `Openssl des3 -d -in I07.des3 -out flag.txt` with password `nakano`

![ss10](https://user-images.githubusercontent.com/101728396/192085640-703765ca-a8ea-41c1-9d8d-a84517944c25.jpg)

![ss11](https://user-images.githubusercontent.com/101728396/192085644-ee5fc2d9-ad1f-491f-972d-86446db69c5e.jpg)

## Question 10
>Find the secret password (flag) of the above-mentioned underground organization!
password: `nakano` and for decrypt des3 using command `Openssl des3 -d -in I07.des3 -out flag.txt`

![ss12](https://user-images.githubusercontent.com/101728396/192085593-a1c324ad-2558-45bf-b3c6-68f5f82af822.jpg)

![ss13](https://user-images.githubusercontent.com/101728396/192085596-dad6aed8-162e-439a-a429-4d67a67269cb.jpg)

### Trouble 
In macOS for number 9 and 10 we cannot decrypt using des3 I dont know why. the output always shown as `bad decrypt` 

On success decrypt

![ss14](https://user-images.githubusercontent.com/101728396/192085598-45c89a8e-061d-4d43-8f90-ab04709bd2d4.jpg)

