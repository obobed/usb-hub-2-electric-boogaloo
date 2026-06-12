# UEB2
## another usb hub!
I made this since I wanted a unique USB hub with cool colours unlike some bland and boring ones you find off Amazon or places like that. It has 2 USB-C, 1 USB-A and an Micro SD card slot for downstream ports, and a USB-C female port for the upstream.

## Repo Structure
When a directory includes a folder named "archive", that contains the files I used before I modified my PCB to use a female upstream port instead of a male one
* [/3D](/3D) - 3D models (both the components and the whole pcb exported as a STEP)
* [/cad](/cad) - my case exported from onshape (you can view the actual onshape link below), has both models with the PCB inside, and without the PCB
* [/images](/images) - various image assets used in my readme (here) and my zine!
* [/pcb](/pcb) - all of my kicad design files
* [/plots](/plots) - various plots, including dxfs for each layer, and a schematic image
* [/production](/production) - contains everything needed for PCB production, like gerbers and a component BOM
* [/rendering](/rendering) - the documents I used in Blender to render my design, with the OnShape exported objs in a subfolder
* [/zine](/zine) - my Zine! pdf and png included, and most assets are in [/images](/images)


## CAD
[OnShape link here!](https://cad.onshape.com/documents/3911889ee056a8d8e4ba98bf/w/b6e308ebfed3eeb37e65c26c/e/fc788076bb25bd97f4780c85?renderMode=0&uiState=6a2ab7df3cd020227a4c42b9)
Step files can be found in [/cad](cad/)

## Images
### Schematic
<img src="/images/schema.png" alt="schematic" width="50%">

### 3D Model
<img src="/images/3D-view-latest-no-receptacle.png" alt="3D front view" width="50%">
<img src="/images/3D-view-back.png" alt="3D back view" width="50%">

### PCB
<img src="/images/full-pcb.png" alt="full pcb image" width="50%">

#### Front Copper
<img src="/images/front-copper.png" alt="front copper pcb image" width="50%">

#### Back Copper
<img src="/images/back-copper.png" alt="back copper pcb image" width="50%">

#### Silkscreen
<img src="/images/front-silkscreen.png" alt="front silkscreen image" width="50%">
<img src="/images/back-silkscreen.png" alt="back silkscreen image" width="50%">

## BOM
### PCB Components
| Designator | Footprint | Quantity | Value | LCSC Part # | Link | Cost ($) |
| --- | --- | --- | --- | --- | --- | --- |
| C1, C4 | 603 | 2 | 4.7u | C19666 | https://jlcpcb.com/partdetail/20375-CL10A475KO8NNNC/C19666 | 0.184 |
| C10, C11, C8 | 402 | 3 | 100n | C1525 | https://jlcpcb.com/partdetail/1877-CL05B104KO5NNNC/C1525 | 0.0345 |
| C12, C9 | 402 | 2 | 1u | C52923 | https://jlcpcb.com/partdetail/53938-CL05A105KA5NQNC/C52923 | 0.069 |
| C13 | 603 | 1 | 1u | C15849 | https://jlcpcb.com/partdetail/16531-CL10A105KB8NNNC/C15849 | 0.079 |
| C14, C15, C2, C6 | 603 | 4 | 10u | C19702 | https://jlcpcb.com/partdetail/20411-CL10A106KP8NNNC/C19702 | 0.346 |
| C3, C5 | 603 | 2 | 100n | C14663 | https://jlcpcb.com/partdetail/YAGEO-CC0603KRX7R9BB104/C14663 | 0.094 |
| C7 | 402 | 1 | 10u | C15525 | https://jlcpcb.com/partdetail/16204-CL05A106MQ5NUNC/C15525 | 0.093 |
| D1 | D_SOD-323 | 1 | 1N5819WS | C191023 | https://jlcpcb.com/partdetail/GuangdongHottech-1N5819WS/C191023 | 0.0555 |
| D2, D3 | UDFN-9_L3.9-W1.1-P0.80-BL | 2 | RCLAMP3328P.TZT | C3040834 | https://jlcpcb.com/partdetail/SEMTECH-RCLAMP3328PTZT/C3040834 | 8.191 |
| D4, D5, D6, D7 | SOD-523_L1.2-W0.8-LS1.6-RD | 4 | PESD5V0V1BB,115 | C477993 | https://jlcpcb.com/partdetail/Nexperia-PESD5V0V1BB115/C477993 | 8.6925 |
| R1, R2, R3 | 603 | 3 | 10k | C25804 | https://jlcpcb.com/partdetail/26547-0603WAF1002T5E/C25804 | 0.021 |
| R10, R7, R8, R9 | 603 | 4 | 56K | C23206 | https://jlcpcb.com/partdetail/23933-0603WAF5602T5E/C23206 | 0.04 |
| R4 | 402 | 1 | 5K1 | C25905 | https://jlcpcb.com/partdetail/26648-0402WGF5101TCE/C25905 | 0.0045 |
| R5, R6 | 402 | 2 | 10k | C25744 | https://jlcpcb.com/partdetail/26487-0402WGF1002TCE/C25744 | 0.028 |
| SIM1 | SIM-SMD_8P-1040310811 | 1 | 1040310811 | C585350 | https://jlcpcb.com/partdetail/MOLEX-1040310811/C585350 | 3.37 |
| U1 | SSOP-16_L4.9-W3.9-P0.64-LS6.0-BL | 1 | GL823K-HCY04 | C284879 | https://jlcpcb.com/partdetail/GenesysLogic-GL823KHCY04/C284879 | 2.2815 |
| U2 | SSOP-16_L4.6-W2.6-P0.53-LS4.0-BL | 1 | SL2.1S | C2684433 | https://jlcpcb.com/partdetail/CoreChips-SL21s/C2684433 | 1.253 |
| USB1, USB3, USB4 | USB-C-SMD_TYPE-C-16PIN-2MD-073 | 3 | TYPE-C 16PIN 2MD | C2765186 | https://jlcpcb.com/partdetail/SHOUHAN-TYPE_C_16PIN_2MD_073/C2765186 | 1.1776 |
| USB2 | USB-A-TH_10.0QHHTZB6.3 | 1 | 10.0 QHHTZB6.3 | C668591 | https://jlcpcb.com/partdetail/SHOUHAN-10_0_QHHTZB63/C668591 | 0.4634 |

### Others
| Item | Quantity | Link | Cost ($) | Notes |
| --- | --- | --- | --- | --- |
| Heatset inserts | 3 | https://www.aliexpress.com/item/1005006967339727.html | 3.00 |  |
| 3D Printed Case | 1 |  | FREE (if you have a printer) |  |
| PCB | 5 | jlcpcb.com | 4.00 |  |
| PCBA | 2 | jlcpcb.com | 47.54 |  |
| PCB Shipping | 1 | jlcpcb.com | 1.50 |  |
| Acrylic | 1 | https://www.mclaser.com.au/products/acrylic-frosted | $9.50 | the other options with smaller sizes were based in another state, and had like $10 shipping, while I am able to pick this up for free. also u can probably find something cheaper on aliexpress |
