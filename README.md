# Custom keyboard
It all started with my dad getting arthritis, which is a genetic disease causing pain in the articulations. However, it can be minimized and even prevented, thus why I started to look into ergonomic 
keyboards between other things to take care of my articulations since young. \
Warning: This takes time to adjust if you want to join the niche of small keyboards because it works with layers, all the keys are there but you use them switching layer or with a combo of strokes.\
<img width="1600" height="897" alt="WhatsApp Image 2026-09-15 at 23 48 27" src="https://github.com/user-attachments/assets/c1919d89-fa88-49cb-b85e-70862aa7a600" />


## Step 1: Investigation
There were a lot of ergonomic keyboards in the market, all of which very expensive. So I decided to build my own based on a repository I found "tompi/cheapino", which I used as the base and configured for my hand size and preferences.

## Step 2: PCB and electronics
I downloaded tompi's pcb design and slightly modified it's lenghts to suit my hand. I decided to keep the author's signature "Chapino" for recognition as my edit was minimal.\
In these builds usually 2 MCUs are used but in this case it only uses one, an RP2040-Zero with 29 data ports, it's not enough for the 36 keys of the keyboard, thus why it uses a matrix pattern, some pins for 
row others for column we have enough for the 36 keys, and both halves (it's a split keyboard) are connected via RJ45 (classic ethernet cable). Cheap, simple and reliable.\
The volume and in my case brightness too are controlled my a potentiometer that works as an extra key.

## Step 3: Shopping list
As this is a personal project and nothing professional I don't wanna look into all the components used and it's link to aliexpress but this is the list:\
- PCBs from PDBWay
- Potentiometer
- Potentiometer cover
- RJ45 ports and cable
- RP2040-Zero
- MCU sockets (for swapping without desoldering in case it fries or has a fault)
- Diodes
- Keycaps
- Hot-swaps for the keys
- Keys (I got classic browns)
- Rubber stickers to prevent sliding
- Type-C cable (I used an old phone's cable)
Total: 67.90€ for 2 keyboards and spare pieces.
Note: You need soldering equipment which I already had.

## Step 4: Mounting process
I built it following tompi's guide, it's quite simple just solder the diodes in it's correct direction, the hot-swaps, the potentiometer, the RJ45s and the MCU. Then insert the keys and keycaps 
and the potentiometer's cover. Connect everything together and now the fun part.

## Step 5: Firmware
For the keyboard to work you have to boot a firmware into the MCU, it can be done easily in the web "vial.rocks". I'll upload my configuration so that you can take a peek.
