# SeedSigner Plus Display Hat

## Supporting the Project
If you are producing these to sell, please consider donating <TBC> per board to <TBC> to support the project.

## Design Files
The files used to produce the original SeedSigner+ hat can be found in the `designspark_format` folder. This also includes production files that can be used to have the board fabricated.

A version in KiCAD format can also be found in the `kicad_format` folder along with all he files needed for low-cost economic fabrication with JLCPCB. (Very low cost if you are happy have one side assembled and manually solder the buttons on)

## LCD Display

The current design assumes LCD available here: https://www.alibaba.com/x/B1E3wJ

**LCD Specifications**
Size: 2.8 inch
LCD Type: IPS (A TFT cheaper TFT panel will work, but has a smaller viewing angle)
Outline Dimensions: 47.8*66.95*2.13mm
Number of Dots: 240(RGB)*320
Controller: ST7789
PIN NO.: 40P
Display Color: RGB565
Backlight: White LED
Polarizer Mode: Transmissive
Data Interface: 3/4-Wire SPI interface, MCU 8/16Bit interface
Operating Temp.: -20 ~ 70 degree
Storage Temp.: -30 ~ 80 degree
Viewing Direction: 12 O’clock / Full

**Pinout for Display**
| PIN | Symbol        | Notes                                                     |
| --: | ------------- | --------------------------------------------------------- |
|   1 | XL / X−       | Resistive touch X− electrode (if resistive touch is used) |
|   2 | YU / Y−       | Resistive touch Y− electrode                              |
|   3 | XR / X+       | Resistive touch X+ electrode                              |
|   4 | YD / Y+       | Resistive touch Y+ electrode                              |
|   5 | GND           | Ground                                                    |
|   6 | VDD           | Logic supply voltage (typically 3.3 V)                    |
|   7 | VDD           | Logic supply voltage (typically 3.3 V)                    |
|   8 | TE            | Tearing Effect output (optional, frame sync signal)       |
|   9 | CSX / SPI_CS  | Chip Select for SPI or parallel interface                 |
|  10 | DCX / SPI_SCL | Data/Command select (SPI clock in SPI mode)               |
|  11 | WRX / SPI_DCX | Write strobe (parallel) or Data/Command in SPI            |
|  12 | RDX           | Read strobe (parallel interface only)                     |
|  13 | SPI_MOSI      | SPI Master Out / Slave In                                 |
|  14 | SPI_MISO      | SPI Master In / Slave Out                                 |
|  15 | RESX          | Hardware reset (active low)                               |
|  16 | GND           | Ground                                                    |
|  17 | DB0           | Parallel data bus bit 0                                   |
|  18 | DB1           | Parallel data bus bit 1                                   |
|  19 | DB2           | Parallel data bus bit 2                                   |
|  20 | DB3           | Parallel data bus bit 3                                   |
|  21 | DB4           | Parallel data bus bit 4                                   |
|  22 | DB5           | Parallel data bus bit 5                                   |
|  23 | DB6           | Parallel data bus bit 6                                   |
|  24 | DB7           | Parallel data bus bit 7                                   |
|  25 | DB8           | Parallel data bus bit 8                                   |
|  26 | DB9           | Parallel data bus bit 9                                   |
|  27 | DB10          | Parallel data bus bit 10                                  |
|  28 | DB11          | Parallel data bus bit 11                                  |
|  29 | DB12          | Parallel data bus bit 12                                  |
|  30 | DB13          | Parallel data bus bit 13                                  |
|  31 | DB14          | Parallel data bus bit 14                                  |
|  32 | DB15          | Parallel data bus bit 15                                  |
|  33 | LED-A         | Backlight LED anode (usually requires current driver)     |
|  34 | LED-K         | Backlight LED cathode                                     |
|  35 | LED-K         | Backlight LED cathode                                     |
|  36 | LED-K         | Backlight LED cathode                                     |
|  37 | GND           | Ground                                                    |
|  38 | IM0           | Interface mode select (sampled on reset)                  |
|  39 | IM1           | Interface mode select (sampled on reset)                  |
|  40 | IM2           | Interface mode select (sampled on reset)                  |

**Note: The Pin numbering on the FPC connector is in reverse order to the list above**
