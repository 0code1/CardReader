# A Nøgle
***
### Description 

this project is support to help the key system we have in skp about the A(Alternative) key.
since peapol need to register an application form manuelly with paper and pen everytime they 
borrow the key. The object of this system is to make it more autonomous and faster.
so that peapol doen't wast time to write  down the form.
the form contain:

1. the name of the borrower (user).
2. where it will be use (location).
3. at what time it were borrow.
4. then peapol will have to check out when the key is return.
5. there must be a website with a log where the instructore will be able to check in case of need

***

### Overview of the project

After some throught of the project.
<br>
The projekt will be made with an Adruino wish will display  a menu via an LCD with the help of a keypad
peapol will be able to choose the option of the key location.
<br>
To register the peapol we will use an rfid reader that will be able to r/w  to a database
<br>
and there will be need of a website for the administration instructor  to check  in case of need. there for we will need some log  in the database


***

### Material

1. LCD display
2. Keypad
3. RFID
4. Adruino mega2560
5. Atmel ice
6. protenciometer
7. database
8. website

***
### Pogram used

- AtmelStudio : c programming for embbeded
- Tera Term   : Console terminal for embbeded testing
- Visualstudio: for fullstack programing

***
## Important informattion and documentation
***
#### Arduino Datasheet 

https://ww1.microchip.com/downloads/en/devicedoc/atmel-2549-8-bit-avr-microcontroller-atmega640-1280-1281-2560-2561_datasheet.pdf

#### Arduino Pinout Diagrram

![Pinout](Billede/MEGApinout.jpg)

##### LCD DATASHEET

https://www.sparkfun.com/datasheets/LCD/HD44780.pdf

##### LCD Usefull information

http://maxembedded.com/2011/06/lcd-interfacing-with-avr/ <br>
this is link referrence will be the closest one to the one we will use on the project with a lcd library, information about installation, and coding sample for our lcd will be here  
<br>
https://www.electronicwings.com/avr-atmega/lcd16x2-interfacing-with-atmega16-32 <br>
This link is an advance version, with the basic  on how the lcd is build without the library  

#### Keypad DATASHEET

https://www.parallax.com/sites/default/files/downloads/27899-4x4-Matrix-Membrane-Keypad-v1.2.pdf


***

## Start Project

***

### Project HIPO Diagram

![akeyhipo](Billede/AKeyHipo.png)

***

## LCD 

***

#### Interfacing Diagram

![IDiagram](Billede/LCD_diagram.png)

This picture is from Ilearn, the pin to the adruino are not like in the picture 

#### Wiring Diagram

![WDiagram](Billede/Wiring.png)

This picture is from Ilearn, the pin use in this picture are different from the one we are using take that in mind

#### LCD Documentation

We will be using  a library for our LCD, the library we will be using is from<br>
https://ilearn.eucsyd.dk/mod/resource/view.php?id=166719<br>
In case of not having acceces to the skole Ilearn or the page above, the original one is  posted here:<br>
https://www.avrfreaks.net/projects/lcd?module=Freaks%20Academy&func=viewItem&item_id=997&item_type=project

In this project we will be using the **PORT A**  on Arduino Mega2560 with the following Pin:

- pin 0 for DB7
- pin 1 for DB6
- pin 2 for DB5
- pin 3 for DB4
- pin 4 for RW
- pin 5 for D/W
- pin 6 for E

#### TODO
- [x] DataSheet
- [x] Interfacing Diagram
- [x] Wiring diagram
- [x] Documentation

***

## Keypad

***

#### TODO

- [ ] HIPO
- [ ] Flow Shart
- [ ] Make it work with interrupt
- [ ] Return a string instead of a char
- [ ] Display the  menu on keypad click:
    - Lager
    - Faverihallen
    - Oslo
    - X-feldt
    - Møbellageret
    - Madrid
    - Post
    - Andet
- [ ] lock function when key on use


***

## RFID

***

#### TODO

- [ ] Check how is work
- [ ] Test with a skole card
- [ ] HIPO
- [ ] Flow Shart
- [ ] Try to communicate with AD/DB
- [ ] Check database for card
- [ ] Get user name of the card ID code
- [ ] desplay username on the LCD
- [ ] BLock other user to use card while the key is out
- [ ] Unblock when the same card is rescaned

***

## Database

***

#### TODO

- [ ] Check if there is any DB or AD that have the card record
- [ ] How to connect to the AD/DB from  an Arduino
- [ ] How to read/write to a database with Arduino
- [ ] Check encoding (hashing and salting)
- [ ] Look for possibility for best practice (no decryption/decode when data return)

***

## Webiste

***
#### TODO
- [ ] research (option) :
    - possibility to have it on one of our earlier website ex: (astrow) , (intra) or other
    - if not make a new one

***

