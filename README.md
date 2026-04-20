# InkTime Smartwatch — PCB Design

InkTime este un smartwatch open-source si low-cost, cu ecran e-paper.

## Diagrama bloc

<img width="816" height="695" alt="image" src="https://github.com/user-attachments/assets/9d18757b-c435-4918-83f6-a35668b2f1a6" />


## BOM (Bill of Materials)

| Referinta    | Componenta               | Descriere                        | JLC Parts                                                                    | Datasheet                                                                                                   |
| ------------ | ------------------------ | -------------------------------- | ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| U1           | nRF52840-QIAA            | MCU principal BLE 5.0            | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=nRF52840)           | [Datasheet](https://infocenter.nordicsemi.com/pdf/nRF52840_PS_v1.7.pdf)                                     |
| IC9          | RT6160AWSC               | DC/DC Buck-Boost 3.3V            | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=RT6160AWSC)         | [Datasheet](https://www.richtek.com/assets/product_file/RT6160A/DS6160A-00.pdf)                             |
| IC1          | BQ25180YBGR              | LiPo Charger                     | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=BQ25180)            | [Datasheet](https://www.ti.com/lit/ds/symlink/bq25180.pdf)                                                  |
| U3           | MAX17048G+T10            | Fuel Gauge I2C                   | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=MAX17048G)          | [Datasheet](https://datasheets.maximintegrated.com/en/ds/MAX17048-MAX17049.pdf)                             |
| IC3          | BMA421                   | IMU Accelerometru 3 axe          | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=BMA421)             | [Datasheet](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bma421-ds000.pdf) |
| IC2          | DRV2605YZFR              | Haptic Driver I2C                | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=DRV2605)            | [Datasheet](https://www.ti.com/lit/ds/symlink/drv2605.pdf)                                                  |
| ANT1         | 2450AT18B100E            | Antena Bluetooth 2.4GHz          | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=2450AT18B100E)      | [Datasheet](https://www.johansontechnology.com/datasheets/2450AT18B100E/2450AT18B100E.pdf)                  |
| J1           | 503480-2400              | Conector display e-paper 24 pini | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=503480-2400)        | [Datasheet](https://www.molex.com/pdm_docs/sd/5034802400_sd.pdf)                                            |
| J4           | KH-TYPE-C-16P            | Conector USB-C 16 pini           | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=KH-TYPE-C-16P)      | -                                                                                                           |
| D3           | USBLC6-2SC6Y             | Protectie ESD USB                | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=USBLC6-2SC6Y)       | [Datasheet](https://www.st.com/resource/en/datasheet/usblc6-2.pdf)                                          |
| D2, D4, D5   | MBR0530                  | Dioda Schottky                   | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=MBR0530)            | [Datasheet](https://www.onsemi.com/pdf/datasheet/mbr0530-d.pdf)                                             |
| J2           | TC2030-IDC               | Conector SWD Tag-Connect         | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=TC2030)             | [Datasheet](https://www.tag-connect.com/wp-content/uploads/bsk-pdf-manager/TC2030-IDC_1.pdf)                |
| X1           | Crystal 32MHz            | Cristal principal MCU            | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=32MHz+crystal+3225) | -                                                                                                           |
| X2           | Crystal 32.768kHz        | Cristal RTC                      | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=32768+crystal)      | -                                                                                                           |
| L7           | FTC252012SR47MBCA        | Inductor 0.47uH DC/DC            | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=FTC252012SR47)      | -                                                                                                           |
| L5           | Inductor 68uH            | Inductor e-paper drive           | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=68uH+inductor)      | -                                                                                                           |
| L1           | Inductor 3.9nH           | Inductor RF matching             | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=3.9nH+inductor)     | -                                                                                                           |
| L2           | Inductor 15nH            | Inductor RF                      | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=15nH+inductor)      | -                                                                                                           |
| L3           | Inductor 10uH            | Inductor DC/DC                   | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=10uH+inductor+0402) | -                                                                                                           |
| Q1           | DMG2305UX-7              | MOSFET P-channel e-paper         | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=DMG2305UX)          | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf)                                         |
| Q3           | SI1308EDL-T1-GE3         | MOSFET N-channel e-paper         | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=SI1308EDL)          | [Datasheet](https://www.vishay.com/docs/71509/si1308edl.pdf)                                                |
| SW_UP/DN/ENT | Butoane tactile SMD      | 3 butoane fizice                 | [JLC](https://jlcpcb.com/parts/componentSearch?searchTxt=tactile+button+smd) | -                                                                                                           |
| R*, C*       | Rezistente/Condensatoare | Diverse valori pasive            | [JLC](https://jlcpcb.com/parts)                                              | -                                                                                                           |

---

## Descrierea functionalitatii hardware

### Microcontroller — nRF52840 (U1)

Nucleul dispozitivului este **nRF52840** de la Nordic Semiconductor, un SoC cu procesor ARM Cortex-M4 la 64MHz si BLE 5.0 integrat. Acesta coordoneaza toate perifericele prin interfetele SPI, I2C si GPIO.

Antena externa **ANT1** (2450AT18B100E) este o antena ceramica de 2.4GHz plasata la marginea dreapta a placii. Sub antena exista un decupaj in PCB pentru a maximiza performanta RF — FR4-ul absoarbe semnalul daca antena sta direct pe el. Circuitul de adaptare RF include inductorii L1 (3.9nH), L2 (15nH) si condensatoarele C3, C4, C22.

**Interfete folosite:**

- **SPI** → display e-paper (J1): MOSI, SCK, CS, DC, RST, BUSY
- **I2C** → IMU (IC3), charger (IC1), haptic (IC2), fuel gauge (U3), DC/DC (IC9)
- **USB** → D+/D- prin protectie ESD D3
- **SWD** → programare/debug prin J2 (TC2030-IDC)
- **GPIO** → butoane, intreruperi IMU, HAPTIC_EN

### Alimentare

**IC1 (BQ25180YBGR)** — charger LiPo care preia alimentarea de la USB-C si incarca bateria. Comunica cu MCU prin I2C pentru statusul incarcarii.

**IC9 (RT6160AWSC)** — DC/DC buck-boost converter care genereaza **3.3V stabil** din tensiunea bateriei (3V–4.2V). Inductorul L7 (0.47uH) face parte din circuitul de comutare. Condensatoarele C23, C24 filtreaza intrarea si C25, C33 iesirea.

**U3 (MAX17048G+T10)** — fuel gauge care monitorizeaza nivelul bateriei prin I2C si trimite o intrerupere (ALERT) la nRF cand bateria scade sub un prag configurat.

Bateria se conecteaza direct la test pad-urile **TP_VBAT** si **TP_BAT_GND** (fara conector JST) pentru economisire de spatiu.

### Display e-paper — J1 (503480-2400)

Conector FFC ZIF cu 24 de pini. Circuitul de drive include Q3, Q1, L5 (68uH), D2, D4, D5 si condensatoarele EPD_C1...C12. Comunicatie prin **SPI** + GPIO de control.

### IMU — BMA421 (IC3)

Accelerometru triaxial Bosch conectat prin **I2C**. Folosit pentru wake-on-wrist, pedometru si detectie orientare. Intreruperile IMU_INT1/INT2 sunt conectate la GPIO-uri dedicate ale nRF.

### Haptic — DRV2605YZFR (IC2)

Driver de motor haptic controlat prin **I2C**, activat prin **HAPTIC_EN**. Suporta efecte LRA si ERM din biblioteca interna de 123 efecte.

### USB-C — KH-TYPE-C-16P (J4)

Conector USB-C cu protectie ESD asigurata de D3 (USBLC6-2SC6Y). R1_USB si R2_USB (5K1) pe pinii CC1/CC2 pentru detectia cablului USB.

### Programare SWD — TC2030-IDC (J2)

Conector Tag-Connect 6 pini pentru programare si debug SWD. Semnale: SWDIO, SWDCLK, RESET, SWO, 3.3V, GND.

---

## Pinii nRF52840 folositi

| Pin nRF52840  | Semnal    | Componenta             | Functie                       |
| ------------- | --------- | ---------------------- | ----------------------------- |
| P0.00 (XL1)   | XL1       | X1 (32MHz)             | Cristal principal — clock MCU |
| P0.01 (XL2)   | XL2       | X1 (32MHz)             | Cristal principal — clock MCU |
| P0.26         | SCL       | IC3, IC1, IC2, U3, IC9 | I2C clock                     |
| P0.27         | SDA       | IC3, IC1, IC2, U3, IC9 | I2C data                      |
| P0.13         | D-        | J4 via D3              | USB Data minus                |
| P0.14         | D+        | J4 via D3              | USB Data plus                 |
| P0.17         | EPD_RST   | J1                     | Reset display e-paper         |
| P0.18 (RESET) | RESET     | J2                     | Reset MCU via SWD             |
| P0.19         | EPD_BUSY  | J1                     | Status display e-paper        |
| P0.20         | EPD_DC    | J1                     | Data/Command display          |
| P0.21         | EPD_CS    | J1                     | Chip select display SPI       |
| P0.22         | SCK       | J1                     | SPI clock display             |
| P0.23         | MOSI      | J1                     | SPI data display              |
| P0.24         | SWDCLK    | J2                     | SWD clock programare          |
| P0.25         | SWDIO     | J2                     | SWD data programare           |
| P1.01         | HAPTIC_EN | IC2                    | Enable haptic driver          |
| P1.02         | PMIC_INT  | IC1                    | Intrerupere charger           |
| P1.03         | IMU_INT1  | IC3                    | Intrerupere IMU 1             |
| P1.04         | IMU_INT2  | IC3                    | Intrerupere IMU 2             |
| P1.05         | SW_UP     | SW_UP                  | Buton sus                     |
| P1.06         | SW_ENT    | SW_ENT                 | Buton enter                   |
| P1.07         | SW_DN     | SW_DN                  | Buton jos                     |
| ANT           | RF        | ANT1                   | Antena Bluetooth 2.4GHz       |
| VBUS          | VBUS      | J4                     | Detectie USB conectat         |
| DEC3V3        | 3V3       | IC9 output             | Alimentare 3.3V               |

---

## Structura PCB

**Dimensiuni:** 46mm x 35mm, grosime 1mm
**Straturi:** 4 (Top + GND + Power + Bottom)

| Strat            | Continut                        | Latime trasee |
| ---------------- | ------------------------------- | ------------- |
| Top              | Componente SMD + semnale date   | min 0.15mm    |
| GND (interior)   | Plan de masa complet            | -             |
| Power (interior) | Trasee 3V3, VBAT, VBUS, VREG    | 0.3mm         |
| Bottom           | Semnale suplimentare + plan GND | min 0.15mm    |

Toate componentele sunt plasate exclusiv pe stratul **TOP**.

---

## Decizii de design

**Alegerea 4 straturi**
S-a optat pentru 4 straturi datorita densitatii mari de componente si numarului mare de semnale. Stratul interior Power permite rutarea traseelor de alimentare (3V3, VBAT, VBUS) separat de semnale.

**Conectarea GND prin Copper Pour**
Pinii de GND nu au fost conectati manual prin trasee individuale.
In schimb, s-au realizat planuri de masa (copper pour GND) pe straturile
Top, GND interior si Bottom. Prin refill-ul poligoanelor, toate padurile
de GND se conecteaza automat la planul de cupru, eliminand necesitatea
airwires-urilor individuale de GND.

## Erori DRC acceptate

- **Board Outline Clearance (~40 erori)** — cauzate de plasarea butoanelor si mufei USB conform specificatiilor mecanice. Neglijate conform enuntului proiectului.
- **"Only INPUT pins on NET ID"** — ignorata conform indicatiilor din enunt.
- **Erori de Dimension la butoane si USB** — neglijate conform enuntului.
- **Overlap-uri** — in anumite zone foarte aglomerate ale PCB-ului, rutarea semnalelor nu a putut evita complet apropierea de pinii vecini fara a intrerupe conexiunile necesare. S-a acceptat un numar mic de overlap-uri in aceste zone.
- **Fisierul `.fbrd` de referinta furnizat continea deja ~46 de erori DRC** din cauza formei si constructiei componentelor. Acestea nu au putut fi eliminate deoarece tin de geometria placii impuse.
