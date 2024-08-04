Continuing with geolocation CTF now we have this case:

### Operation-Bloodhounded

```
Greetings, Special Agent,

It’s great to hear that your exercise went well, and congratulations to your team for winning. Now, let’s get back to business. Our old friend Maksim Kotova has escaped the Schneider residence under mysterious circumstances, and our field agents did not see anyone leave.

Nevertheless, we are determined to capture him this time, by any means necessary. A few weeks ago, one of our field agents managed to sneak into the residence and attach a GPS tracker and camera device to Maksim’s jacket.

Unfortunately, it seems that Maksim has taken some countermeasures, as the GPS functionality of our device doesn’t seem to work, most likely due to some jamming device he has on him. Nevertheless, our device automatically connects to any public WiFi network in range and uploads the photos it takes.

It is your assignment to use these photos to locate Maksim Kotova. One you do, we will send in one of our top field agent, Ricardo Alvarez, AKA the Bloodhound. He will make short work of Maksim.

As always, Special Agent. Best of luck on this operation.

```

### Material of the case

We only have 5 photos were taken by Maksim's jacket:

1.- ![Evidence 1](https://github.com/user-attachments/assets/29314a02-c7ad-4984-9816-33951cb47d4d)

2.- ![Evidence 2](https://github.com/user-attachments/assets/b0732aec-8992-48b4-be1b-0e219aca8b4e)

3.- ![Evidence 3](https://github.com/user-attachments/assets/fe299762-3023-4cbe-ac7d-91c9a3252ac8)

4.- ![Evidence 4](https://github.com/user-attachments/assets/56e81e39-e4af-4d32-bafa-804e9907a46f)

5.- ![Evidence 5](https://github.com/user-attachments/assets/784cc892-9526-4fac-858d-636cbfc91685)


### Instructions to the case

```
Find where's Maksim using the photos
Sample answer for the flag: new-york-grand-plaza-hotel
```

### Locating Maksim

We start with a reverse search with the first photo to know where Maksim went when he escaped, after doing this we can see the next information: "**Berlin** - **Brandenburg** (airport) Airport The airport in Brandenburg is located on the border with Berlin in the municipality of Schönefeld."

At the first time, it looks like Maksim is in Germany, but it's still too early to affirm he's there, let's search information with the other images to see what we can found.


The second image can't give us much information by the low resolution, we can't see the text and it complicate the things, so the only thing we can do with this image is search points of reference and search similar places with that points

![Evidence 2 edit](https://github.com/user-attachments/assets/5527c02e-ecc1-429f-bb52-ea828cf70a4c)

Let's get focus on that 2 things: Something like bars on the roof and the blue circular roof of the place.

### Possible place
![Clue](https://github.com/user-attachments/assets/3af7c45b-fffa-47ad-b20c-4264d6b16de0)

We founded a place similar with the bars of the second photo, doing a reverse search with this image we can see the next information: "**Ankara Esenboga Airport**, **Türkiye**, An international airport located 28 kilometers northeast of the center of Ankara, the capital of Turkey."
Now we have another possible place: Turkey and Germany but, what is the correct place?

To be able to answer this question, we have to search the shops are in the airport and look if is a place similar like we see with the blue circular roof:

![Coffe](https://github.com/user-attachments/assets/0724be2a-f557-453c-8585-8eba38d4a74b)

Look what we have here: Investigating on the official website of Ankara Esenboga Airport (_https://esenbogaairport.com/en-EN/shop-dine/food-beverage_) we can see a Coffe Shop with the same blue circular roof that we see in the second photo of Maksim, with this information now we can confirm that Maksim was in Ankara Esenboga Airport, Turkey.

### Data collected at this moment
> Maksim was initially at an airport in Berlin, Germany.
> Then he arrived to Ankara Esenboga Airport in Turkey.
> He was in a Coffe Shop.

Now that we know he is in Turkey, the search will be a little easier.


![Evidence 3](https://github.com/user-attachments/assets/d5489aa4-34fe-469d-a92f-e277ce947273)

In the third photo, we can collect more points of reference:

1.- A big white building with points of view with windows on each floor in the right side.
2.- A series of windows in front of the big building.
3.- A signal with the leyend "END" and a text saying "VIP" on the top side with a draw of a coron.
4.- A wall of rocks in the left side.

At the beginning I tried again the reverse search in Google Lens on PC, but I didn't had good results, so I decided to try doing the same search in a cellphone and I got a result very similar with the photo of the case:
![Result](https://github.com/user-attachments/assets/953494a6-f2f8-4063-b222-660835defe2f)

The photo have a link: _https://www.tapu.com/detay/pursaklar-saray-mahallesinde-3-arti-1-daire-21545_


![Tabu](https://github.com/user-attachments/assets/b21df153-08df-4891-bfee-097eb413c3fb)
![Address](https://github.com/user-attachments/assets/737a5e2a-5b85-49b6-a4e9-efa3529eb50d)

The page contain an address of the building, let's search it on Google Maps:


![Building](https://github.com/user-attachments/assets/d62a20e4-7074-47a2-8cbd-7259dec8c702)
We have the location of the building and a coordinates.


The fourth photo is probably the room where Maksim was, since it is a closed place for the moment we can't do much with that photo, I've tried reverse search and I don't get results.

The five photo looks like a balcony, maybe from the room where he was for a while, as with the previous photo, doing a reverse search doesn't work, so I tried with Google Maps using the layers.

We can take points of reference like we done in the second photo:
> A lamp on the right side.
> A big building on the left side, some characteristics are curved shape and a lot of windows.
> A dome with blue roof.
> A street in the background.

Remembering the data we've collected until this moment, Maksim was in Ankara, by the airport Ankara Esenborga, so we can also try to search in Ankara the place of the fifth photo:
![Map](https://github.com/user-attachments/assets/15f48fd9-cdb2-474c-adac-961909caa2dd)

After a long search into Ankara, we can see a similar place with the datas of the Fifth photo, let's see the Hotel since it seems to be the place where the photo was taken:
![Room](https://github.com/user-attachments/assets/543ae57c-3ed3-4c0b-a096-aae7d6a36eb9)

Some users upload their photos and this room looks very similar with the fourth photo, we can confirm than Maksim was in **_Latanya Hotel Ankara_**

Now we have all the data we needed, we can create the flag of the case:

>ankara-latanya-hotel
