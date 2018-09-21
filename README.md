# Xiaomi-Mijia-1080p-2018
Hacking the Xiaomi Mijia 1080p camera (2018 version, white back)

![](/mijia2018.jpg)

# Teardown
Desc | Picture
--- | ---
Getting into the camera is not as easy as before, the whole case is clipped together tight. It is only two pieces. It cannot be unscrewed like the old one. I had to go medieval on it.| ![](/teardown/IMG_20180802_174022.jpg)
There are two holes where it uncliped first. In hindsight, it might be possible to lift the front plastic and force it open. | ![](/teardown/IMG_20180802_174131.jpg)
After some wiggling it is out... The white back of the stand is not part of the camera module. | ![](/teardown/IMG_20180802_174329.jpg)
Better view of the stand. | ![](/teardown/IMG_20180802_195150.jpg)
The SoC is an Ingenic T20. They switched from Grain Media 8135/6S to what the Dafang has. Winbond W25Q128JVSO SPI flash (the ending O is not on the [datasheet](https://www.winbond.com/resource-files/w25q128jv%20revf%2003272018%20plus.pdf)). Chipstar CS8122S audio amp. The serial interface is next to the flash chip (Tx Rx GND GND N/A). I could not interrupt U-Boot by pressing a key.<br/><br/>[bootlog](/bootlog.md) | ![](/teardown/IMG_20180802_174835.jpg)
Realtek wifi on the other side and the IR leds. | ![](/teardown/IMG_20180802_175143.jpg)

# TODO
Hook up the flash chip and read the firmware...
Update: CH341A with the v1.29 software does not seem to know how to read W25Q128JV.
