# benchpowersupply


# What it is

A 500W Variable PSU with real time CC/CV error correction, current clamping, a 16 bit DAC for millivolt and milliamp precision. 

# Why I Made This
Precision power supplies are really cool, and high power power supplies are also really cool, some precision PSUs having milliamp/millivolt precision, and some high power PSUs going upto 2kW, but I couldn't find a single power supply with more than 300W with sub volt precision for under a lot of money, and I've always wanted to design one since they're really impressive, so I did. 

# Pictures
<img width="1360" height="920" alt="image" src="https://github.com/user-attachments/assets/b232371c-281f-498b-9fb7-ba10bf2b237b" />
<img width="603" height="801" alt="image" src="https://github.com/user-attachments/assets/b9b9e64e-4ab0-480b-a41a-2a73cd119593" />
<img width="603" height="801" alt="image" src="https://github.com/user-attachments/assets/540a3c81-04ee-49da-bccf-c0b75da2427e" />
<img width="603" height="801" alt="image" src="https://github.com/user-attachments/assets/1af9fc7d-fa57-45f6-8aa3-dc83de26590d" />
<img width="603" height="801" alt="image" src="https://github.com/user-attachments/assets/f01fedf8-cdf9-49c5-82e8-5262c660b7d2" />
<img width="483" height="488" alt="image" src="https://github.com/user-attachments/assets/aeea97fd-7b0a-4568-8a94-0c8b587f1bfd" />

<img width="710" height="667" alt="image" src="https://github.com/user-attachments/assets/8b5df8c5-8df7-4d36-984f-5e49cbb7797e" />


# BOM

| Item | Purpose | Qty | Cost | Link |
| :--- | :--- | :---: | :---: | :--- |
| **FC4L90R002FER** | CURRENT SENSE CHIP 1% 0.002 OHM | 5 | $13.75 | - |
| **8174** | TERM SCREW 10-32 4 PIN PCB | 4 | $5.56 | - |
| **FCR7350Y** | 4MM PANEL SKT S16N-PC YELLOW | 2 | $15.74 | - |
| **FCR7350B** | 4MM PANEL SKT S16N-PC BLACK | 2 | $15.32 | - |
| **INA238AQDGSRQ1** | IC PWR MONITOR 10VSSOP | 2 | $9.00 | - |
| **411019-01** | CORD 14AWG NEMA 5-15P TO CBL 10' | 2 | $35.12 | - |
| **0190700090** | CONN RING CIRC 14-16AWG #10 | 6 | $1.32 | - |
| **LM5149RGYR** | 800mV~55V Adjustable Step-down DC DC Controller | 2 | $7.96 | [LCSC](https://www.lcsc.com/product-detail/C7528454.html) |
| **LM5164DDAR** | 1MHz Step-down Adjustable 1A Voltage Regulator | 2 | $0.00 | [LCSC](https://www.lcsc.com/product-detail/C477928.html) |
| **ESP32-S3-WROOM-1-N4** | 2.4GHz ESP32-S3 On-board PCB Antenna Module | 2 | $8.30 | [LCSC](https://www.lcsc.com/product-detail/C2913197.html) |
| **ADS8681IRUMR** | SPI 4.75V~5.25V WQFN-16 Analog to Digital Converter | 2 | $19.80 | [LCSC](https://www.lcsc.com/product-detail/C2670107.html) |
| **REF6025IDGKR** | Series Voltage Reference IC Fixed 2.5V ±0.05% | 2 | $11.72 | [LCSC](https://www.lcsc.com/product-detail/C2157015.html) |
| **DAC8562SDGSR** | 10us 2.7V~5.5V Digital to Analog Converter | 2 | $21.98 | [LCSC](https://www.lcsc.com/product-detail/C127965.html) |
| **INA241A4IDR** | -5V~110V 100V/V Instrumentation / Current Sense Amp | 2 | $7.11 | [LCSC](https://www.lcsc.com/product-detail/C22427873.html) |
| **TLV3501AIDR** | Rail-to-Rail Input/Output SOP-8 Comparator | 2 | $7.00 | [LCSC](https://www.lcsc.com/product-detail/C43484.html) |
| **SER2915H-223KL** | 30A 22uH ±10% Shielded Inductor SMD | 2 | $17.71 | [LCSC](https://www.lcsc.com/product-detail/C19276066.html) |
| **BSC027N10NS5** | N-Channel 100V 3W Surface Mount MOSFET | 2 | $9.80 | [LCSC](https://www.lcsc.com/product-detail/C534315.html) |
| **BSC040N10NS5** | 100V 86A 139W Surface Mount MOSFET | 2 | $1.96 | [LCSC](https://www.lcsc.com/product-detail/C534334.html) |
| **AP2112K-3.3TRG1** | 3.3V Positive Fixed LDO Regulator (TECH PUBLIC) | 5 | $0.00 | [LCSC](https://www.lcsc.com/product-detail/C23380830.html) |
| **AP2112K-3.3TRG1** | 3.3V Positive Fixed LDO Regulator (DIODES) | 5 | $0.00 | [LCSC](https://www.lcsc.com/product-detail/C51118.html) |
| **CC0805KRX7R9BB104** | 100nF ±10% 50V Ceramic Capacitor X7R 0805 | 20 | $0.39 | [LCSC](https://www.lcsc.com/product-detail/C49678.html) |
| **CL21B104KBCNNNC** | 100nF ±10% 50V Ceramic Capacitor X7R 0805 | 20 | $0.30 | [LCSC](https://www.lcsc.com/product-detail/C1711.html) |
| **CL21B105KBFNNNE** | 1uF ±10% 50V Ceramic Capacitor X7R 0805 | 20 | $0.81 | [LCSC](https://www.lcsc.com/product-detail/C28323.html) |
| **0805B222K500NT** | 2.2nF ±10% 50V Ceramic Capacitor X7R 0805 | 20 | $0.12 | [LCSC](https://www.lcsc.com/product-detail/C36576.html) |
| **CC0805JRNPO9BN560** | 56pF ±5% 50V Ceramic Capacitor NP0 0805 | 50 | $0.66 | [LCSC](https://www.lcsc.com/product-detail/C113831.html) |
| **HGC0805R5475K500NSLJ** | 4.7uF ±10% 50V Ceramic Capacitor X5R 0805 | 10 | $0.49 | [LCSC](https://www.lcsc.com/product-detail/C7472969.html) |
| **CL21A106KAYNNNE** | 10uF ±10% 25V Ceramic Capacitor X5R 0805 | 20 | $1.60 | [LCSC](https://www.lcsc.com/product-detail/C15850.html) |
| **0805CG101J500NT** | 100pF ±5% 50V Ceramic Capacitor C0G 0805 | 50 | $0.48 | [LCSC](https://www.lcsc.com/product-detail/C82028.html) |
| **HGC0805R5476M100NSLJ** | 47uF ±20% 10V Ceramic Capacitor X5R 0805 | 5 | $0.81 | [LCSC](https://www.lcsc.com/product-detail/C19103846.html) |
| **1210B104K251CT** | 100nF ±10% 250V Ceramic Capacitor X7R 1210 | 10 | $0.59 | [LCSC](https://www.lcsc.com/product-detail/C304007.html) |
| **EFVH100ADA101M10C0** | 100uF ±20% 100V Aluminum Electrolytic Capacitor | 5 | $1.15 | [LCSC](https://www.lcsc.com/product-detail/C22387799.html) |
| **CL21B102KBCNNNC** | 1nF ±10% 50V Ceramic Capacitor X7R 0805 | 20 | $0.30 | [LCSC](https://www.lcsc.com/product-detail/C46653.html) |
| **2N7002** | N-Channel 60V 115mA 200mW MOSFET SOT-23 | 50 | $0.56 | [LCSC](https://www.lcsc.com/product-detail/C916396.html) |
| **FRC0603F8872TS** | 88.7kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.27 | [LCSC](https://www.lcsc.com/product-detail/C2999456.html) |
| **FRC0603F1072TS** | 10.7kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.23 | [LCSC](https://www.lcsc.com/product-detail/C5153968.html) |
| **RC0603FR-07100KL** | 100kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.23 | [LCSC](https://www.lcsc.com/product-detail/C14675.html) |
| **FRC0603F3163TS** | 316kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.23 | [LCSC](https://www.lcsc.com/product-detail/C2998125.html) |
| **FRC0603F4703TS** | 470kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.21 | [LCSC](https://www.lcsc.com/product-detail/C2907040.html) |
| **HoJLR2512-3W-5mR-1%** | 5mΩ 3W Current Sense Resistor ±1% 2512 | 5 | $0.45 | [LCSC](https://www.lcsc.com/product-detail/C2903482.html) |
| **FRC0603F6193TS** | 619kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.13 | [LCSC](https://www.lcsc.com/product-detail/C5713292.html) |
| **RC0603FR-0710KL** | 10kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.35 | [LCSC](https://www.lcsc.com/product-detail/C98220.html) |
| **FRC0603F1502TS** | 15kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.22 | [LCSC](https://www.lcsc.com/product-detail/C2906995.html) |
| **AR05BTCW4003** | 400kΩ ±0.1% 125mW 0805 Thin Film Resistor | 20 | $0.94 | [LCSC](https://www.lcsc.com/product-detail/C3013969.html) |
| **FRC0603J102 TS** | 1kΩ ±5% 100mW 0603 Thick Film Resistor | 100 | $0.24 | [LCSC](https://www.lcsc.com/product-detail/C2907113.html) |
| **FRC0603J472 TS** | 4.7kΩ ±5% 100mW 0603 Thick Film Resistor | 100 | $0.21 | [LCSC](https://www.lcsc.com/product-detail/C2907166.html) |
| **RS-03K2701FT** | 2.7kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.20 | [LCSC](https://www.lcsc.com/product-detail/C118394.html) |
| **HRC0603F5101ENTN** | 5.1kΩ ±1% 100mW 0603 Thick Film Resistor | 100 | $0.12 | [LCSC](https://www.lcsc.com/product-detail/C54920932.html) |
| **1RC0603J0101** | 100Ω ±5% 100mW 0603 Thick Film Resistor | 100 | $0.17 | [LCSC](https://www.lcsc.com/product-detail/C54531636.html) |
| **EC11E15244B2** | Through Hole Encoder | 4 | $9.59 | [LCSC](https://www.lcsc.com/product-detail/C470754.html) |
| **SMMS0650-680M** | 1.5A 68uH ±20% Molded Inductor SMD | 5 | $0.89 | [LCSC](https://www.lcsc.com/product-detail/C2894721.html) |
| **SMPS** | 600W 60V SMPS PSU | 1 | 31.99 | [Amazon](https://www.amazon.com/NUOWEIDE-Converter-Transformer-Controller-Electric/dp/B0FTYPPZPR/ref=sr_1_5?sr=8-5)


