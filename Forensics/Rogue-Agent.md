The first case of Forensics

### Rogue-Agent

```
Greetings Special Agent.

We have a request on our hands from our friends over at the CIA. In September of 2021, one of their operatives went missing in action. Upon further investigation, it was discovered this operative went rogue and started a smuggling business for the Russians. Mostly dealing in complex electronics, which have become difficult to come by for Russians after sanctions began.

The agent we’re looking for is named Valentino Maggi. Born in Brooklyn New York on 18.05.1987. Valentino is one of five sons of the Valentino family, who moved to the United States during World War II. Having grown up a middle class lifestyle, his father a car salesman and mother working as an elementary school teacher. Valentino was recruited into the CIA during his time as a student at Columbia University.

Most of his 10 years in active service were spent as an analyst working out of Langley. Recently though, in August of 2020, Valentino moved to oversees work. Being stationed in Italy as a liaison officer for the Italian foreign intelligence agency “Agenzia Informazioni e Sicurezza Esterna”.

Doing stellar work, right up until the point he went missing. Prompting an extensive investigation into his whereabouts. Documents were eventually found on his computer, recovered using forensics tools to recover deleted files. These indicate a heavy involvement with the Russian underground. Acquiring much needed microelectronics for the Russian government.

And that is where your task begins, Special Agent K. One of the files recovered from Valentino’s computer, is an image with a text file. We believe this to be the current location of Valentino Maggi. Locate the safehouse, so local authorities can raid the premises.

As always, the contract is yours, if you choose to accept.

```

### Material of the case

A photo of the possible location of Valentino:
![safehouse-aerial-rogue-agent](https://github.com/user-attachments/assets/89f4bb23-8cb2-45d9-90ca-d79850b5976a)

You can download the original image on Google Drive (It's recommended use the original photo to analyze better the data): https://drive.google.com/drive/folders/1bJyerOJa-Ip9EeBTNH9tg8chtFHyPqF1

### Instructions to the case

```
Find the location of the photo
Sample answer for the flag: country-town-coordinate
```

### Analyzing the photo

The first thing I've done was a reverse search like I often do with every image, but this time I didn't had good results.

Then I tried checking the metadata of the photo but the only information I've founded was the format file and the resolution of the photo, nothing of these information are useful for the case.

So, we need to use some Linux tools to complete the case:

I'm using Kali Linux for this work in a VM, after I downloaded the photo I use **strings command**.

### About the command

The command "strings" turns files into readable characters, it is useful to analyze the characters and collect data from the file:
![Strings](https://github.com/user-attachments/assets/8e850e94-5f6b-4d24-b844-a79067dd4053)

We'll have a lot of information and strange symbols, but we don't need all characters, we only need the last characters:
![Data](https://github.com/user-attachments/assets/89ade199-6a5d-4e34-b52f-7f7ae1864735)

We copy the text "Zhh\djrljhZdb\`jnphf" and we need another tool to analyze this fragment.


### Cyber-Chef

For those who don't know this tool: Cyber-Chef is a coder and decoder from data, is a tool can be used from their web page or downloading in Desktop.

Cyber-Chef will help us to decode the fragment of the photo we've turned in string. In this case I'm using the web page for the task:
![Result](https://github.com/user-attachments/assets/280b0d36-baf4-4646-b72c-94444ed05792)

I configured the Cyber-Chef with the tool "Magic" and turning on the option "Intensive mode" to do a deep search and get better results, as we can see, the tool gave us a coordinates.


### Searching the coordinates

At the first time, I tried searching the coordinates as the tool gave me, but while I was searching on Google Maps it appeared me a sea, so, I deleted the negative symbol "-" and I search it again:
![Location](https://github.com/user-attachments/assets/26e47289-7e2e-4752-9313-f38ef01e3923)

And we founded the location of the photo: The city is Rakinac and it's located on Serbia, now we can make the flag:

> serbia-rakinac-44.259654-21.057843
