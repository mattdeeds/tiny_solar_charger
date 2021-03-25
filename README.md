# Tiny Solar Charger
Less than one inch square solar charging board based on the bq25504 solar harvesting ic with onboard solar cell for low power applications

## Parts 
KXOB25-04X3F-TR: MONOCRYSTL SOLAR CELL 22MW 2.07V 
TI BQ25504: Ultra Low-Power Boost Converter With Battery Management 
### Configuration
Currently configured for single cell li-ion batteries but I've tested it with supercapacitors with voltage ratings over 4.2v

BAT_OV = 4.2v
BAT_UV = 3.0v 

Configuration resistor values: 
- R6 = 4.02M
- R7 = 16M 
- R8 = 4.42M
- R9 = 5.49M
- R10 = 4.22M
- R11 = 5.9M
- R12 = 5.620M
- R13 = 3.830M 
- R14 = 0.619M

### Board Pinout and Overview
<img width="741" alt="Screen Shot 2021-03-25 at 4 25 32 PM" src="https://user-images.githubusercontent.com/29756767/112539031-e0b4a000-8d86-11eb-99f2-4d0721a1aa7a.png">

### Todo/improvements
- Schematic specifies an inductor that I'm not actually using, switched to a higher max current 
- Currently using inductor with 300ma max current, datasheet specifies >300ma 
