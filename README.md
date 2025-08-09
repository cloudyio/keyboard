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

| Item | Count | Price Per Item | Total Cost | Source | Notes |
|------|-------|----------------|------------|--------|-------|
| NRF52840 Development Board | 2 | $2.94 | $4.56 | [AliExpress](https://www.aliexpress.com/item/1005001621678794.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%202.94%21USD%202.94%21%21USD%202.94%21%21%21%402103864c17546871093517142e0f12%2112000016846541261%21ct%21UK%21-1%21%212%210) | Cheap nice!nano |
| 1N4148 DO-35 Diodes | 1 | $1.58 | $1.58 | [AliExpress](https://www.aliexpress.com/item/1005007131309837.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%202.55%21USD%201.58%21%21USD%201.58%21%21%21%402103864c17546871093517142e0f12%2112000039509276484%21ct%21UK%21-1%21%211%210) | Diodes |
| Keycap Set | 1 | $32.47 | $32.47 | [AliExpress](https://www.aliexpress.com/item/1005007511714496.html?spm=a2g0o.detail.0.0.4a7bOK6zOK6zd4&mp=1&pdp_npi=5%40dis%21USD%21USD%2029.94%21USD%2027.74%21%21USD%2027.74%21%21%21%40211b613917543927371393706e2a71%2112000041079406832%21ct%21UK%214899091290%21%211%210) | keycap set, quite good quality and look very nice, most price to performacnce i could find |
| JST battery connector  | 1 | $2 | $2 | [AliExpress](https://www.aliexpress.com/item/1005008970428474.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%201.74%21USD%201.74%21%21USD%201.74%21%21%21%402103864c17546871093517142e0f12%2112000047412491082%21ct%21UK%21-1%21%211%210) | Battery connector, comes with 2 |
| power switch | 1 | $2 | $2 | [AliExpress](https://www.aliexpress.com/item/1005006827258573.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%201.56%21USD%201.56%21%21USD%201.56%21%21%21%402103864c17546871093517142e0f12%2112000038431123036%21ct%21UK%21-1%21%211%210) | Also comes with 2 |
| Reset tactile button | 1 | $0 | $1 | [AliExpress](https://www.aliexpress.com/item/1005006292427731.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%200.41%21USD%200.41%21%21USD%200.41%21%21%21%402103864c17546871093517142e0f12%2112000036636688325%21ct%21UK%21-1%21%212%210) | Again, comes with 2 |
| Lithium Battery 110mAh | 1 | $8 | 8$ | [AliExpress](https://www.aliexpress.com/item/1005009279554068.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%2014.17%21USD%207.79%21%21USD%207.79%21%21%21%402103864c17546871093517142e0f12%2112000048591585127%21ct%21UK%21-1%21%211%210) | Pretty cheap batteries, has the pcb integrated and fits under the dev board to stay hidden 2/pc |
| L+R PCB | 1 | $15.00 | $22.00 | [JLCPCB](https://cart.jlcpcb.com/quote?rand=0.6702360434866385) | Both pcbs, includes customs + shipping |
| Kailh Choc v1 Low Profile Switches | 1 | $38 | 38$ | [AliExpress](https://www.aliexpress.com/item/1005006626760418.html?spm=a2g0o.cart.0.0.272a38daeUtKrN&mp=1&pdp_npi=5%40dis%21USD%21USD%2038.48%21USD%2038.48%21%21USD%2038.48%21%21%21%402103864c17546871093517142e0f12%2112000040228314274%21ct%21UK%21-1%21%211%210&pdp_ext_f=%7B%22cart2PdpParams%22%3A%7B%22pdpBusinessMode%22%3A%22retail%22%7D%7D) | Pretty good switches for a good price, only need 60 since keyboard is 58 keys |
| Black fillament | 1 | $18 | $18 | [Amazon](https://a.co/d/5nH2rc7) | Grey fillament thats cheap, only one i could find in budget |
| Heat inserts | 1 | $1.70 | $1.70 | [AliExpress](https://www.aliexpress.com/item/1005008666672949.html?spm=a2g0o.productlist.main.1.ca0120e5XnvkcI&algo_pvid=65c3fc17-1755-45b7-85bb-becc4f9a3a66&algo_exp_id=65c3fc17-1755-45b7-85bb-becc4f9a3a66-0&pdp_ext_f=%7B%22order%22%3A%222513%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21USD%211.85%210.99%21%21%211.85%210.99%21%402103835e17543530241436264e5646%2112000046157335300%21sea%21UK%210%21ABX&curPageLogUid=fu29zqBtC1Cv&utparam-url=scene%3Asearch%7Cquery_from%3A) |  Heat inserts so fillament doesnt get destroyed, they annoyingly only come in 50 but there cheap so its fine anyway |
|  |  |  | $130.42 |  |  |
notes:

- VAT is included but shipping is not since it varies, will typically end up at arround 7-15 dollars


