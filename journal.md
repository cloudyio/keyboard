---
title: "Cloudboard"
author: "Cloudy"
description: "A small low profile keyboard!"
created_at: "2024-06-14"
---
# June 14th: 

I did basic research on what goes into making a low profile keyboard and the differences when designing it, i decided on a wired keyboard since i want it to be small and it is generally just easier to design a wired one, i also found a 75% to be the best for me. Picture of layout below:

![keyboard layout](static/layout.jpg)

**Total time spent: 1h**

# June 16th: 

Did more research and resetup kicad, i looked through a bunch of boards and found the nice!nano, the nice!nano honestly seemed great for the build but costing arround 30$ for a microcontroller seemed like a bad idea, i went back to look for another board and ended up finding this:

[Supermini NRF52840](https://www.aliexpress.com/item/1005006019812115.html)
This is a really good alternative to the nice nano, it is considered Nice!Nano compatible meaning any info i find on the nice!nano will be relevant to this board, also significantly cheaper then the other board coming in at ￡7.79

One of the main reasons i really like this board is the fact it is bluetooth and has charging managment, making my life much easier and brings bluetooth back as an option.

I also did look for a dongle reciver and stumbled across the [nRF52840 Dongle](https://www.nordicsemi.com/Products/Development-hardware/nRF52840-Dongle), it is zmk compatible which is one of the main reasons its good but i dislike the bulkyness and think ill keep looking
 
**Total time spent: 1h**

# June 26th: 

Designed the schematic in kicad and changed the layout

![image](https://github.com/user-attachments/assets/54e04a13-ca16-484a-a316-b7c9fabad227)

the new layout adds more functionality and buttons but im stuck on how i am going to fit the dev board on the new design, i also created the key layout schematic in kicad:

![image](https://github.com/user-attachments/assets/1099d48f-1dad-449c-86c4-4a9eedbea567)

but the dev board i am using has one less gpio pin to what i need so i either need to pick a dev dev board, not use a dev board at all or optimise the matrix more.
i also researched some stiff on the material and came to the realisation that having my case cnc'd would be way to expensive. So right now i am planning on 3d printing it with a unique stratergy with nylon using a 3d printing method called MJF, i think it will come to arround 60 dollars but i can only tel when my case is done

 
**Total time spent: 3h**

# June 28th: 

I came to the realisation that a dev board just wouldnt fit and the keyboard wouldnt be as compact as a wanted if i wanted to use one, so i am now embedding the microcontroller on to the pcb. I started with adding a usb c receptacle but kept hitting more and more issues as i went along, i ended up with this after 3 hours of work:
![image](https://github.com/user-attachments/assets/951d871c-306b-4faf-9934-6873b9cfbd35)
What i tried to do was use a IC to controll the battery so the battery wasnt charging all the time and the keyboard could either be wired or wireless, i also plan to use a 2 pin battery connector in case i ever need to replace the battery. Overall it has been very overwhelming and ill come back to it later because im 80% sure it wont work. I am now also using [ai03s guide](https://wiki.ai03.com/books/pcb-design) to try and simplify what i need to do.

 
**Total time spent: 3.5h**

# July 2nd

Still working on embedding the microcontroller, found ai03s guide very helpful and ended up with this
![image](https://github.com/user-attachments/assets/abb69542-b32d-42d4-b5f2-d0158aa3131a)
This was great progress and everything seemed like it worked, the guide was very helpful at explaining what things did and what to do next but i quickly ran into the issue of running out of gpio pins, the microcontroller i was using (ATmega32U4) just didnt have enough pins unless i wanted to optimise my matrix. This really wasnt great as i wanted to make designing the pcb itself after the schematic as easy as possible and didnt want routes all over the place.

I then decided on the rp2040 which had enough io pins for the layout i wanted. I found [this guide](https://www.youtube.com/watch?v=6Z49bynRqj8) very helpful at the begining as it showed how to correctly wire the microcontroller with the crystal and flash memory along with a usb c port. After following i ended up with this:

![image](https://github.com/user-attachments/assets/65e42489-c10c-43fe-9881-d0c592a2ff3c)

# July 6th

Havent posted a log for a while because it has been very on and off, i have pretty much decided on the FINAL mcu i will use for the keyboard, the [MDBT50Q-1MV2](https://www.raytac.com/product/ins.php?index_id=24), it has everything i need like a built in antenna and a usb interface making my life so much easier. Appart from that it has just been integrating everything from past designs into one complete circuit, making this:

![image](https://github.com/user-attachments/assets/cda1ce9f-f60c-43e5-9b92-c5c24900e7f2)

**Total time spent: 2h**


# July 9th

Ive been working on routing the pcb and have got to this point:

![image](https://github.com/user-attachments/assets/746a65f4-d387-4fd9-ad34-a9e556f622ae)

This is great progress for me and the pcb is fully complete now, unless i add drill holes later. The keyboard uses a GND filled zone, this is to make the routing neater in general and can help with heat. Ive puposefully moved all the smd parts to the back since i am planning on getting them assembled, this is due to me not being skilled enough at soldering to properly soldier the parts properly. 3d render of the pcb:

![image](https://github.com/user-attachments/assets/e9b3f331-8471-423b-885c-5c324a73ab2e)

Getting the board assembeled might be expensive though. just on jlcpcb alone your required to assemble at least 2 boards which quoted me at arround 50 dollars for 2 assembled boards, 3 empty.

**Total time spent: 3h**







