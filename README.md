# Jarkom-Modul-1-I07-2022

Group Members:
1. Denta Bramasta Hidayat (5025201116)
2. Ghazi
3. Rivaldo


## Question 1
Mention the website server used on “monta.if.its.ac.id”? 

answer: `http.host contains monta.if.its.ac.id`

[ss]

## Question 2
Ishaq was confused looking for TA topics for this semester, then he came to the monta website and found the topic details on the website “monta.if.its.ac.id”, what TA title did Ishaq open?

answer: `ip.host == 103.94.189.5 && tcp contains detailTopik`

[ss]

## Question 3
Filter so that wireshark only shows packets going to port 80!

answer: `display filter tcp.dstport == 80 || udp.port == 80`

[ss]

## Question 4
Filter so that wireshark only picks up packets coming from port 21!

answer: `tcp.srcport == 21 || udp.srcport == 21`

[ss]

## Question 5
Filter so that wireshark only picks up packets coming from port 443!

answer: `tcp.srcport == 443 || udp.srcport == 443`

[ss]



