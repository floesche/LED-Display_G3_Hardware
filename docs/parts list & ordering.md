
# Parts list
(Goal: includes pictures of each item and instruction for any custom ordering)

## Controller components

### Main controller board
order from Bittele: JF‐MR‐PC0003 RevC _2018_05_25 (updated with more details! ask Will)

### BNC breakout 
order bare PCB from pcbcart.com, then solder in below parts

geber file: panels_bnc_breakout_v1p1.zip  (TODO link to file in repo!)
board size: 203.2mm x imm
layers: 2
board type: single
material details: FR4-Standard Tg 140C
thickness (finished board): 1.6 mm
surface finish: HASL
soldermask: As design in file
solder mask color: green
copper weight (finished): 35 um
silkscreen legend: as design in file
silkscreen legend color: white
see PCB quote screenshot for other options (pcb_cart_quote_screenshot.png)
![pcb_cart_quote_screenshot](https://user-images.githubusercontent.com/4358857/115049775-12fa7e80-9ea9-11eb-903e-9dac7e4f96e3.png)
    
Panels BNC Breakout BOM:
| Part   |      Description      |  Vendors |
|----------|:-------------:|------:|
| P1,P2 |  5x2 male shrouded header | jameco 67812,  digikey S9169-ND |
| P3 |    4-pin friction lock header   |   jameco 613958, digikey A1922-ND |
| P4-P13 | socket BNC connector |    digikey A97555-ND  |
| P14 | 13x2 male shrouded header |  jameco 68372,  digikey S9173-ND |
    

### ISP breakout 
order bare PCB from pcbcart.com, then solder in below parts
geber file: panels_isp_breakout_v1p1.zip
board size: 25.4mm x 35.56mm
see PCB quote screenshot for other options (pcb_cart_quote_screenshot.png)
     
Panels ISP Breakout BOM:
| Part   |      Description      |  Vendors |
|----------|:-------------:|------:|
| P1 |  8pin receptacle 0.1"  | digikey SAM1222-08-ND |
| P2 |     friction lock header 0.1"   |   digikey A1922-ND |
| P3 | 3x2 male header 0.1" |    digikey WM8121-ND  |
| R | resistor 10k, 1/4W 5% |  digikey P10KBACT-ND |


### Enclosure
Purchase 300mm deep 1U rackmount blank chasis from: https://www.circuitspecialists.com/rackmount-enclosure-37-1u.html

Hardware for connecting PCBs, see below (Enclosure Hardware)
Power supply: Digi-Key 1939-1462-ND

Enclosure Hardware:                     

Qty    Description                                  Vendor             Part Number
----------------------------------------------------------------------------------------
1      panel switch                                 Digi-Key           CH865-ND   
8      4-40 standoff - 3/8" long                   McMaster-Carr      91780A730  
16     4-40 screws 1'4" long                       McMaster-Carr      91249A105  
4      nylon unthreaded spacer                      McMaster-Carr      94639A620  
4      4-40 screw, 1'2" long                       McMaster-Carr      91249A111  
1      DC Power Jack panel mount                    MCM Electronics    27-5867    
1      25-pos D-sub connector (blue)                Jameco             12335      
1      Jumper Wire - 0.1", 4-pin, 12"             Sparkfun           PRT-10374  
1      Jumper Wire - 0.1", 2-pin, 12"                 Sparkfun           PRT-10372  
1      Ribbon cable, 25 conductor (5”)                Jameco             643621   
1      Ribbon cable, 10 conductor (7.25” and 12”)   Jameco             643794
1      Cable mount connector, 13 x 2 Position       Jameco             32564      
4      Cable mount connector, 5 x 2 position        Jameco             32492
1          Jumper                       Digi-Key           S9001-ND
1      Male DC 2.1mm x 5.5mm pigtail barrel plug socket adapter Amazon


## Arena components

Qty Description
1   Arena board
1   Arena power supply 5V 30A supply     Jameco PN 123394   https://www.jameco.com/z/S-150-5-MEAN-WELL-AC-to-DC-Power-Supply-Single-Output-5-Volt-30-Amp-150-Watt_123394.html?CID=MERCH
1   Supply to Arena cable (5-pin DIN cable)             http://www.digikey.com/products/en?keywords=839-1064-nd
1   AC power cord                           https://www.mcmaster.com/#70355k85/=16vbkrs
4   Digi-Key    478-4170-ND
14  Digi-Key    SAM1222-08-ND
1   Digi-Key    609-1478-ND
1   Digi-Key    CKN1513-ND
1   Digi-Key    CP-2350-ND
1   Digi-Key    A26513-40-ND
4   Digi-Key    S9001-ND



## Additional equipment
-soldering station
-AVR ISP programmer for programming bootloader and firmware onto controller (https://www.amazon.com/Compatible-System-Programmer-interface-XYGStudy/dp/B00C7VV6E4/ref=pd_sim_147_2?_encoding=UTF8&pd_rd_i=B00C7VV6E4&pd_rd_r=bb50105e-7a32-11e8-b7c4-af38c36f552b&pd_rd_w=0BdWm&pd_rd_wg=x0vvW&pf_rd_i=desktop-dp-sims&pf_rd_m=ATVPDKIKX0DER&pf_rd_p=7967298517161621930&pf_rd_r=WRS771ZEM7MYHXQ577N2&pf_rd_s=desktop-dp-sims&pf_rd_t=40701&psc=1&refRID=WRS771ZEM7MYHXQ577N2)





