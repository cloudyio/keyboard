# Cloudboard

![image](https://github.com/user-attachments/assets/d89a52b3-8189-44c9-9ff8-1f11f88b464c)

A low profile ergo keyboard inspired by the lily 58.

## Overview

The cloudboard is a small low profile keyboard made to be wireless and bluetooth, it features a lily 58 key layout, 110mAh batteriea im each half and 2 supermini controllers

The keyboard uses ZMK for its firmware due to how simple but effective it is for ergo and bluetooth keyboards.

## Why i made the project

Ive wanted to try out a ergo keyboard for a while now and thought it would be a fun idea to make one with the features i actually want and none of the extra parts.

## Features:

### Simple design

The keyboard is made to be clean and compact with each half only being less then 15cm long, the layout used is also concidered a intro ergo keyboard layout having many similarities to a normal layout which makes it easy to learn!

![image](https://github.com/user-attachments/assets/e24635f4-9091-40d6-8df4-e172e8bf7eeb)
*Dev board risen to represent height of header*

![pcb](static/pcb.png)


### NRF52840 Board

The nice!nano is conciderably one of the best boards for a ergo split keyboard, this is due to its small size while still packing bluetooth compatibility, built in battery managment and USB C. One of the biggest issues with the board though is its 20 dollar price point so instead the keyboard uses a replicate alternative which includes **all** the features of the nice!nano (can be found in BOM below).

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/997e4fce-30fc-4af8-adf2-69cb36a1dc38" />


TLDR:

The dev board allows for bluetooth, usb c and battery managment for less than 4 dollars.

### Low profile

Low profile keyboard are better ergonimically, are smaller, lighter and arguably look better. The keyboard features choc v1 switches to give the board a even lower size profile and sound profile.

![image](https://github.com/user-attachments/assets/4c022ef0-c3ee-48b4-a293-6787055a77df)




## BOM

| Item                               | Count | Price Per Item | Total Cost  | Source                                                                                          | Notes                                                                                                              |
| ---------------------------------- | ----- | -------------- | ----------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| NRF52840 Development Board         | 2     | $2.28          | $4.56       | [AliExpress](https://www.aliexpress.com/item/1005006343285322.html)                             | Cheap nice!nano                                                                                                    |
| 1N4148 DO-35 Diodes                | 1     | $1.03          | $1.03       | [AliExpress](https://www.aliexpress.com/item/1005002339916163.html)                             | Diodes                                                                                                             |
| Keycap Set                         | 1     | $29.94         | $29.94      | [AliExpress](https://www.aliexpress.com/item/1005007511714496.html)                             | keycap set, quite good quality and look very nice, most price to performacnce i could find                         |
| JST battery connector              | 1     | $1.00          | $1.00       | [Typeractive](https://typeractive.xyz/products/battery-jack?variant=45597492707559)             | Battery connector, comes with 2                                                                                    |
| Power switch                       | 1     | $2.00          | $2.00       | [Typeractive](https://typeractive.xyz/products/power-switch?variant=45597854171367)             | Also comes with 2                                                                                                  |
| Reset tactile button               | 1     | $2.00          | $2.00       | [Typeractive](https://typeractive.xyz/products/reset-button?variant=45597784932583)             | Again, comes with 2                                                                                                |
| Lithium Battery 110mAh             | 2     | $4.00          | $8.00       | [Typeractive](https://typeractive.xyz/products/lithium-battery-110mah?variant=43294731665639)   | Pretty cheap batteries, has the pcb integrated and fits under the dev board to stay hidden                         |
| Sockets and Pins                   | 2     | $7.00          | $13.00      | [Typeractive](https://typeractive.xyz/products/machine-sockets-and-pins?variant=45741664501991) | Hot swap pins, makes the dev board easy to take off the pcb in case of issues, also adds height for battery        |
| L+R PCB                            | 1   | $23           | $23    | [JLCPCB](https://cart.jlcpcb.com/quote?rand=0.6702360434866385)                                 | Both pcbs                                                                                                          |
| Kailh Choc v1 Low Profile Switches | 6     | $6.00          | $33.00      | [Typeractive](https://typeractive.xyz/products/choc-switches?variant=45741919240423)            | Pretty good switches for a good price, only need 60 since keyboard is 58 keys                                      |
| Black fillament                    | 1     | $18.00         | $18.00      | [Amazon](https://a.co/d/5nH2rc7)                                                                | Grey fillament thats cheap, only one i could find in budget                                                        |
| Heat inserts                       | 1     | $1.70          | $1.70       | [AliExpress](https://www.aliexpress.com/item/1005008666672949.html)                             | Heat inserts so fillament doesnt get destroyed, they annoyingly only come in 50 but there cheap so its fine anyway |
|                                    |       |                | **$144.76** |                                                                                                 |                                                                                                                    |
|                                    |

notes:

- VAT is included but shipping is not since it varies, will typically end up at arround 7-15 dollars
- most parts picked from typeractive for conviniece since it has the keycaps and switches + most components needed and also to keep shipping costs low
- Typer active has an active 5% discount code as of making it, making it even cheaper
