### On-the-wire

```
Greetings Special Agent.

One of our field agents in Malaysia managed to physically breach the office of a corrupt politician. Doubling as a mole for a Chinese criminal enterprise, mostly smuggling endangered animals. In this case their evil business involves shark fin trade and other exotic food items.

During the breach, our agent successfully obtained several pieces of information on the organization. Currently this does not include their name, as they only communicate using anonymous messages and codenames.

We hope that the information, which includes pictures, floorplans, data dumps and packet captures. Will lead to a more complete picture of this organization. We know that the Malaysian government will be exceptionally happy to get this criminal enterprise out of its borders.

All data has been divided over several agents. Your segment for this contract is the analysis of a packet capture file. Figure out what is being communicated and find the message that matters.

As always, the contract is yours, if you choose to accept.
```

### Material of the case

You can download the .pcapng file here: _https://drive.google.com/drive/folders/1muDbw7c0fMosl5BqTbadHAIjZe-GXD98_


### Instructions to the case

```
Analyze the traffic and find something useful to the case about illegal animals exportations
```

### Analizing the traffic
To this case, we need a sniffer software, I'll use *Wireshark* to analyze the traffic. So, first we need to download the file and load it in the software:
![Captura 1](https://github.com/user-attachments/assets/de6867ce-c278-4ba4-81a5-f1179ab88314)

It is worth remembering that traffic analysis is a time-consuming job that requires a lot of patience, we need to see first all the protocols was used in the traffic. And after a while, I founded various protocols: TCP, TLS v1.2, TLS v1.3, DNS, and QUIC

The protocol DNS looks interesting, so I put DNS filter on Wireshark and started to analyze all packages that contains DNS:

![Capture 2](https://github.com/user-attachments/assets/15ffa189-d112-4d6d-aaf9-558d6831a5fe)

Checking the packages we can see the user had visited search engines, Microsoft and Google services, social media, etc. But after a long time seeing all the packages I founded something interesting:
![imagen](https://github.com/user-attachments/assets/38891d21-46c3-4565-9dec-2d53544dc350)

The user visited a pastebin, for those who don't know the pastebin: Is a web application where people can upload small texts, is more used to upload code, links, etc.

The cybercriminal use pastebins to upload their malicious links and store their data leaks, or hide their content to go unnoticed around the world.

Here is the link: _https://pastebin.com/raw/U7zb8Kyh_


If we open the pastebin it give us the next Bit.ly URL: _https://bit.ly/3qyrf7t_

And we founded a clue to the case of the corrupt politician, unfortunately the URL has been deactivaded, I tried following the URL putting "+" symbol at the end to see where it redirects but I couldn't do it:
![Error](https://github.com/user-attachments/assets/2a537915-2c3a-4f4e-8700-ced0ae3803f8)

At least we founded the flag for the challenge:

> https://bit.ly/3qyrf7t
