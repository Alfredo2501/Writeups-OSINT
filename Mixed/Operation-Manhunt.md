Continuing with the story of Maksim Kotova:

### Operation-Manhunt

```
Maksim Kotova has escaped from the ICC prison in Scheveningen, the Netherlands. Given Russia’s current need for weapons, and Kotova’s connections to get those weapons, we can only assume he’s had help from his fellow countrymen.

On Monday 26.12.2022 at exactly 03:30, Maksim Kotova was picked up by an armored transport vehicle, to be taken to the US embassy in Wassenaar. As the truck waited for the embassy entrance to open, six armed gunmen blew out the back door, eliminated all security personnel and extracted Maksim Kotova in a VW Golf.

They sped off in Western direction, being recorded on two traffic camera’s as they made a run for the beaches of Scheveningen. At the beach, they were picked up by a RHIB that took them out into the fog. As reported by three eye witnesses who were walking their dog’s on the beach.

The Dutch Coast Guard and Koninklijke Marechaussee (Military Police) searched coastal waters all day and called for assistance from the British Royal Navy, being the next likely waters to enter. All this led to nothing but annoyed fishermen as their ships were boarded.

Fast forward to today, in cooperation with INTERPOL, our Red Team codenamed “Echo” was able to gain access to an IRC channel used by the Order of Hades. Which led to an email address of an informant becoming known to us. Which Echo then used to spoof and convince an agent handler inside the Order of Hades to provide information about Maksim Kotova.

The information is a sock puppet Twitter account, used by Kotova to post information about his whereabouts. His handler uses this information to infer if Maksim is doing okay. All to prevent any actual communication between members of the Order of Hades. Under the guise of a generic tourist in some foreign country.

It is your task to monitor the Twitter account and piece together enough information to locate Maksim Kotova. Be careful not to interact with the account in any way, nor with the accounts it follows. Use the posted information to geolocate Kotova and relay the information to me.

As always, Special Agent, the contract is yours, if you choose to accept.

```

### Material of the case

Sock puppet profile: https://x.com/mkultrabanger
In case of X delete the account you can see a photo of the profile on the original Google Drive Hacktoria of CTF: https://drive.google.com/drive/folders/17qDKEOkLOFJwYRhIqEXU9e4t4dT0NjOw


### Answer instruction
Lowercase letters and hyphens only
English language used for locations on Google Maps
Total character count: 53
Amount of hyphens: 7


### Instructions to the case

```
Find where's Maksim using the information on his sock puppet
Sample answer for the flag: my-country-city-beautiful-street-trioli-awesome-hotel
```

### Analizing X account
Let's see the x account of Maksim, it should be remembered that it is strictly **prohibited** to interact with the profile in any way. So we can't send messages, like photos or publications, leave a comment, etc. Social engineering cannot be used in this case.

So the only way we have to search information is looking all the publications in the profile.

To make the search a little easier, we can take as a reference information about the case and take the date when Maksiwm escaped in the VW Golf: 12/26/2022, so, we can search publication nearby date:
![Capture 1](https://github.com/user-attachments/assets/81470264-4465-44e4-8132-23681784963b)

The account started his publications 1 day after he escaped, let's see the other publications:
![Capture 2](https://github.com/user-attachments/assets/40d6b1f3-b142-4a26-911a-f50ecedbab52)

We can take this publications as a keywords and references:
* The photo can mean he's nearby on a beach, a river, a lake, or another place where are water.
* The other publication he said "yachts" and "bay".
* In the photo he said "Hotel", so our answer will be a hotel.

### Reverse search

![imagen](https://github.com/user-attachments/assets/fe9b03fb-6092-4af2-84e9-66350fdf109d)

We have a photo of a beach and he said in another publication "beach" and again "bay". That reinforces our keywords and references.

Let's do a reverse search of this photo and let's see if we can find something useful:
![Results](https://github.com/user-attachments/assets/cd86a425-4345-4ca5-806c-a8edac105b41)

This image looks similar of the Maksim's photo, let's see the Web Page:
![Web](https://github.com/user-attachments/assets/39817907-4a8f-4c7b-bfbb-7b242a0aaa0f)

We have the name of the beach "Sao Vicente Baia Das Gatas", let's search it on Google Maps:
![Maps](https://github.com/user-attachments/assets/8e9f2b20-5ec1-40cc-ac4a-0be4c1a1ff85)


### Using our keywords and references
Just having the name of the beach isn't enough information to locate Maksim, so, we can use our keywords to search an approximate location.

Remember he said "Yachts" and "Bay", also he said "Hotel", so let's start searching hotels nearby of Das Gatas:
![Hotels](https://github.com/user-attachments/assets/e78a0518-92e0-4c72-93e6-219dc7890df7)

We have a lot of results, and where we have to search?, easy.

Remembering the photo of the beach in Maksim's profile, he said "_A short drive to check this place out_", the place of the photo Das Gatas, so he traveled a short distance to arrive to the beach, which means he's in a hotel nearby of Das Gatas, let's get focused in nearby hotels.

![Nearby result](https://github.com/user-attachments/assets/ddd022f6-5c24-4b65-bad2-934c218c978d)
Using our keywords, we must focus in hotels near of the sea.


After a long search in all the hotels, the result with more coincidences is **Georgette Hotel**:
![Georgette](https://github.com/user-attachments/assets/3c9ba297-889f-4928-9fe8-c385d3442a7e)

We found the hotel where Makism is, now to finish we just need the address of the hotel: "Avenue Marginal, Copacabana Mindelo São Vicente, 2110, Cabo Verde"

> cape-verde-mindelo-ave-marginal-georgette-guest-house
