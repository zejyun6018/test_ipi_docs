# SCDP Introduction

<br>

<br>


 ![image-20210820140603168](introduction.assets/image-20210820140603168.png)

<br>

​                                                                                                                                 <img src="introduction.assets/image-20210820111800694.png" alt="image-20210820111800694" style="zoom:67%;" />

​                                        

<br>

<br>



## System Components

- COM HPC module with 32-core ARM based Ampere Altra SOC
- COM HPC Server carrier
- Intel Quad X710 10GbE Lan Card
- USB 3.0 Card for Front panel
- 32 GB DDR4 System Memory
- 128 GB NVMe M.2 storage 
- Tower Enclosure
- Liquid cooling assembly
- 750 Watt Power Supply



<br>

<br>

### COM HPC ALT module

<br>

#### Introduction

COM HPC ALT is a Computer on Module based on the PICMG COM HPC Server type open standard, it measures 200mm x 160mm. 
On the back side it has two 400 pin high-performance connectors, for a total  of 800 pins interconnects with a carrier board. 

The COM-HPC Server Type targets use in high-end headless (no display) embedded servers that require intensive CPU capability, large memory  capacity, and lots of high bandwidth I/O including multiple 10Gbps or  25Gbps Ethernet, and up to 65 PICe lanes, at up to PCIe Gen 5 speeds. Typical uses are in embedded server equipment ruggedized for use in field environments and applications such as autonomous vehicles, cell  tower base stations, geophysical field equipment, medical equipment,  defense systems, and much more. 

Server Modules use fixed voltage 12V input power. Server Modules can accept up to 358W of input power (using the connector vendor recommended 20% current capacity derating) over the 28 Module VCC pins, at the low end of the 12V power in range. This allows CPUs with up to about 175W dissipation to be deployed on Server Modules. The limit is subject to considerations such as the connector pin derating used, the number of memory sockets used, and other power consumers on the Module.

The COM HPC ALT module is a commercial of the shelve type of component (COTS) that can be paired with custom designed carrier to facilitate different industrial verticals.COM HPC ALT is revision controlled and offers production lifetimes in excess of 10 years.  Computer on module design are widely accepted in the embedded world and drastically lower a customer's time to market and total cost of ownership (TCO)

More information about the COM HPC formfactors can be found here : 

https://www.picmg.org/openstandards/com-hpc/

<br>

<br>

<br>



 ![image-20210820111800694](introduction.assets/image-20210820111800694.png) 

<br>

<br>

 ![COM HPC ALT front side](introduction.assets/COM-HPC-ALT_F_Final-1-1.jpg)



COM HPC ALT front side

<br>

 ![COM HPC ALT back side](introduction.assets/COM-HPC-ALT_B_final-1.jpg)


COM HPC ALT back side

<br>

<br>

<br>

#### A1 Function Diagram

<br>

 ![Function Diagram](introduction.assets/image-20210808170652562.png)






<br>

<br>

<br>

#### Ampere Altra SOC

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![image-20210820163240550](introduction.assets/image-20210820163240550.png) | ●   32 Arm v8.2+ 64-bit CPU cores up to 1.7 GHz with Sustained Turbo <br />●   SBSA Level 4<br />●   64 KB L1 I-cache, 64 KB L1 D-cache per core <br />●   1 MB L2 cache per core 32 MB System Level Cache (SLC) <br />●   2x full-width (128b) SIMD Coherent mesh-based interconnect<br />    – Distributed snoop filtering<br /> |

<br>

<br>

<br>

### COM HPC Server Carrier

COM HPC Server carrier is a general purpose carrier for generic COM HPC server type modules typically used for prototyping purposes. 

The carrier an EATX size and can be mounted into standard EATX capable tower enclosures.

It is powered by off the shelve ATX type power supplies 

<br>

 ![COM-HPC Carrier Board](introduction.assets/COM-HPC Carrier Board-F.jpg)
<br>


<br><br>


#### Function Diagram



![image-20210820115045673](introduction.assets/image-20210820115045673.png)

<br>

<br>

#### Interfaces

<br>

| PCIe slots                 | Rear I/O                               | Aux Headers          |
| -------------------------- | -------------------------------------- | -------------------- |
| PCIe x16 GEN4  two slots   | 4x USB 4.0 on rear I/O                 | RS232                |
| PCIe x8 GEN4 one slot      | LAN GbE on rear I/O                    | 5x FAN power         |
| PCIe x4 GEN4 two slots     | LAN GbE on rear I/O for BMC management | Front panel signals  |
| M.2 PCIe x4 GEN4 two slots | Analog VGA on rear I/O                 | SPI, GPIO, I2C       |
|                            | RS232 DB9 on rear I/O                  | 2x SATA (not active) |

<br><br><br>

### Quad 10GBASE-T LAN card

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Intel Ethernet Controller XL710 <br /><br />4x 10GBase-T RJ45 Standard <br /><br />Cat6a Cabling with RJ45 Connectors up to 100 meters <br /><br />Autonegotiation between 100Mb/s, 1GbE and 10GbE PCIe 3.0 x8<br /> | ![PCIe Quad 10GbE ](introduction.assets/image-20210820123103468.png) |

 


<br>

<br><br>

### USB 3.0 Card for Front panel 

|                                                              |                                                           |
| ------------------------------------------------------------ | --------------------------------------------------------- |
| ● NEC / Renesas D720201 chipset card<br /><br />● supporting 4 USB 3.0 connection totally<br />  - 2x back USB 3.0 ports<br />  - 1x 20-pin USB 3.0 header  supporting up to 2 USB 3.0 on front panel<br /><br /><br /> | ![usb 3.0 CARD](introduction.assets/41ysMkpiRoL._AC_.jpg) |

<br>

<br>

<br>

### Tower Enclosure

<br>

![Tower Enclosure](introduction.assets/image-20210808165218496.png)


<br>

 <img src="./introduction.assets/image-20210808165301005.png" alt="image-20210808165301005"  />

 <br>

<br>

<br>

### Liquid Cooling Assembly

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ● Asetek  based all-in-one closed loop, maintenance free liquid cooling solution for Ampere Altra SOC<br /><br />● All aluminum radiator with 11 water channels to disperse water and heat.<br /><br />● Thermally optimized cooling plate and low-noise pump design for high performance, quiet cooling<br /><br />● Two 120 mm Vento ARGB fans | ![usb 3.0 CARD](introduction.assets/image-20210820124355271.png) |

<br>

<br><br>

### ATX Power Supply

|                                                              |                                                |
| ------------------------------------------------------------ | ---------------------------------------------- |
| ● 80 Plus Gold Certified <br/>● ATX Version : ATX 12V V2.52     <br />● Protection : OCP / OVP / UVP / OPP / SCP / OTP / NLO / SIP<br/>● Certifications : CE / UKCA / CB / FCC (IC) / EAC / CCC / TUV / cTUVus / RCM / NOM / BSMI / KC<br />● PFC : 0.99<br/>● Input Voltage : 100-240V<br/>● Input Frequency : 47Hz-63Hz<br />● Noise Level @ 20% : 11.2dB(A)<br/>   Noise Level @ 50% : 750W : 11.3dB(A) <br/>   Noise Level @ 100% :  750W : 22.7dB(A)<br/>● EPS 8 (4+4) Pin Connector  : 750 Watt<br /> | ![](introduction.assets/productGallery174.png) |





