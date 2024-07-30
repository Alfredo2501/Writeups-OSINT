In this case, we have the next message:

### Caged-Princess

```
Greetings, Special Agent. 

It has come to our attention that one of our subsidiaries, crucial for reconnaissance operations, has fallen victim to a ransomware attack. This incident has disrupted our ongoing mission in the Riviera region. Although the impact on our overall operations is minimal, we require your expertise to investigate this breach and ensure the security of our digital infrastructure. 

Your mission, should you choose to accept it, is to conduct a thorough investigation into the ransomware attack. You will need to identify the threat actor behind this attack, assess the extent of the damage, and determine how much sensitive data has been compromised. It is imperative that you trace the origin of the attack but also maintain Operational Security as you may become a target yourself. 

To aid in your investigation, you will be provided with minimal details regarding the cyber attack. Our Hacker Dimitri will be available to assist you as needed. Once you have gathered sufficient information and have a clear understanding of the situation, you are to provide a detailed report of your findings back to SERPENT HQ. Time is of the essence in this matter, as we cannot afford any further disruptions to our operations. We have complete faith in your abilities to handle this situation with the utmost professionalism and discretion. 

As always, the contract is yours, if you choose to accept. 

```

### Materials

Only we have a few keywords to the case:

> Monaco 2023
> Ransomware

### Instructions

```
Find who was the victim of the attack, the group who made the attack, and the size of information robbed.
Sample answer for the flag: company-name-threat-actor-data-amount-exfiltrated (GB at the end of the amount-exfiltrated not required)
```

### OSINT to the Ransomware
First I've tried with Google Dorks, but I didn't have good results with that.

So I had to search in fonts more focused with ransomware attacks like: *https://www.ransom-db.com/*

Using "Monaco" as Keyword, I got 2 results:
![Capture](https://github.com/user-attachments/assets/584affe6-cb12-411a-ad84-0ec2b9430fe7)

We'll get focus on the attack that have date as "2023"
Now we have a few datas will help us:
> **_Monaco-Technologies_** (Name of victim)
> **_Lockbit 3.0_** (Name of attacker)

Now we only need the size of information robbed, we can make a search in Google using the keywords now we have: "monaco-technologies ransomware"
and we found the next link: *https://hackmanac.com/news/hacks-of-today-09-10-11-09-2023*

In this compilation of business that had suffered a ransomware attack, Monaco Technologies appears on the list with the next information:
![Monaco](https://github.com/user-attachments/assets/01a21302-84f5-4b5f-917c-ad68f9b7e998)

We have the same information we found on the previous page, but now we have the size of information robbed: 
> **_23.7_**

Now we have all the data we need and now we just have to make the flag:

> **_monaco-technologies-lockbit3.0-23.7_**

