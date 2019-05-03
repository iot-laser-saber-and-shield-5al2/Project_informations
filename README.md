# Laser Saber and Shield - Project informations


## Description

`Laser Saber and Shield` consists of making a representation of a fighting game with lightsabers and shields. The goal is to make a fight between two people and the person who is the most affected, lost the fight.


## Get started

### Arduino step

* Download [Arduino](https://www.arduino.cc/en/Main/Software).

* Set this `Additional Boards Manager URLs` (`File -> Preferences`) in your Arduino IDE: `http://arduino.esp8266.com/stable/package_esp8266com_index.json`

* Go to `Tools -> Board Type -> Board Manager` and install the following packages: `esp8266` and `WiFi Manager`

### Processing step

* Download [Processing](https://processing.org/download/).

* Go to `Sketch -> Import Library... -> Add Library...` and install the following libs: `oscP5`, `sound` and `controlP5`

### Cloning step

* `git clone https://github.com/iot-laser-saber-and-shield-5al2/Server`
* `git clone https://github.com/iot-laser-saber-and-shield-5al2/Firmware`

### Start step

1. Use an hotspot WIFI
2. Change firmware WIFI parameters 

![WIFI_parameter](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/WIFI_parameters.png)

3. Assembly hardware

![Assembly hardware](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/HardwareBis.jpg)

4. Upload Firmware into hardware
5. Make your sword

![Assembly hardware](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/HardwareFinal.jpg)

7. Start your server *(The server may take a long time to launch depending on the size of the files.)*

8. START TO FIGHT !!!


## Hardware infos

| Reference | Product | Unit Price** | Qty | Total |
| --------- | ------- | ---------- | --- | ----- |
| ESP8266 | [Espressif ESP8266 Microcontroller](https://www.amazon.fr/Crazepony-UK-NodeMcu-Development-ESP8266-ESP-12F/dp/B06XPCR921/ref=sr_1_10?__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=ESP8266&qid=1556881498&s=gateway&sr=8-10) | 7€ | 2 | 14€ |
| GY521 | [Module MPU-6050 3 axes Gyroscope + Accelerometer](https://www.amazon.fr/SODIAL-MPU-6050-Gyroscope-Accelerometre-Arduino/dp/B00K67X810/ref=sr_1_2?__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=GY521&qid=1556881561&s=gateway&sr=8-2) | 2€ | 2 | 4€
| MAX7219 | [8-Digit LED Display](https://www.amazon.fr/Hiletgo-daffichage-contr%C3%B4le-Electronic-Production/dp/B00LSG54O2/ref=sr_1_19?__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=MAX7219&qid=1556881650&s=gateway&sr=8-19) | 3€ | 2 | 6€ |
| - | [Fake sword](https://www.amazon.fr/Vileda-107931-Universel-Plastique-Multicolore/dp/B002IJM40A/ref=sr_1_3?keywords=Manche+%C3%A0+balai&qid=1556881359&s=gateway&sr=8-3) | 1.50€ | 2 | 3€ |
| - | [External battery](https://www.amazon.fr/Anker-Batterie-PowerCore-Technologies-VoltageBoost/dp/B01CU1EC6Y/ref=sr_1_10?__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=power+bank&qid=1556882479&s=gateway&sr=8-10) | 10€ | 2 | 20€ |
***Price is as an indication, you can find a cheaper one.*

![Espressif ESP8266 Microcontroller](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/ESP8266.jpg)

![Module MPU-6050 3 axes Gyroscope + Accelerometer](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/GY521.jpg)

![8-Digit LED Display](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/MAX7219.jpg)

![Fake sword](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/balai.jpg)

![External battery](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/ExternalBattery.jpg)

## Project board

Trello link : <https://trello.com/b/zL0Afcey/iot>

## More informations

### Introduction
 
Our subject is a fighting game using lightsabers. The goal is to make a fight between two people and the loser is the one that got hit the more.

Here are the rules of the fight: Hit the opponent to inflict damage until he has no life left. The winner is the one with the most points of life. Each participant has a sword and the goal is to inflict damage to his opponent and the first one below 0 health point has lost.

### Installation
 
It is necessary to install the Arduino software as well as Processing. Arduino allows you to implement an embedded code in the connected object. It contains manageable libraries in order to code, compile and test our work. Processing is a graphical interface for communicating with Arduino. This software also contains manageable libraries order to centralize the data coming from the connected object.
 
### Components
 
To successfully develop our project, we used 2 ESP8266 as well as 2 GY-521 to have the frequencies required data necessary for the calculation of the shock threshold.

![ESP8266](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/ESP8266.jpg)

![GY-521](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/GY521.jpg)

Here is the main component fused. It must be inserted in the sword in order to recover the moment of shock.

![IMG COMPLET MODULE](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/HardwareFinal.jpg)

In order to establish some tests with sword strokes, we attached a ESP8266 with a pet to a large bottle of water that is about the size of the sword and we made gestures. We got what we needed from the Arduino Software plot as well as the data.
 
### Resources
 
We needed two Star Wars lightsaber toys.
We have tinkered with the aim of integrating cleanly and without having a problem of attachment or violent impact to the object an ESP8266.
 
We have also integrated the other ESP8266 into the shield. It has also been integrated properly.
 
### Problems encountered

We had several ideas as we went along and we tried to apply them to our project but we were short of time which prevented us from realizing them.

We have not all had experience in electronics. This course represented for us a first experience in the field and we had some difficulties producing this project. In addition, the work is processing and we have not had any experience on 3D representatives.

The definition of shock was not easy to do. We defined the shock mostly thanks to the accelerometer. The calculation of the shock wasn’t simple because of the shock threshold

### The smooth running of the project

We shared the tasks. We have a team that takes care of the lightsaber then, a person who takes care of the documentation. We set up a few things, including a moment of the day dedicated to sharing. Everyone explains to the whole team what everyone has done in order to stay up-to-date with news and share knowledge.

### Possible future improvements 

We had ideas as the project progressed.
We thought of hanging a screen to trigger the score of each player like the MAX7219 and produce a sound of "game over" when the countdown comes to 0.
We also thought to add a shield that will protect the fighters during the duel.
To have more effects during the duel, we thought to add a sensor that captures the impacts which emits a vibration and a sound effect of the type "Star Wars". We thought to reproduce the fight in 3D and to visualize it in the software "Processing"

![MAX7219](https://github.com/iot-laser-saber-and-shield-5al2/Project_informations/blob/master/gallery/MAX7219.jpg)

### Members of the team
 
- FAIRFORT Yohan
- RAMASSAMY Loghan
- SAHRI Hamza
- SMATI Hamza
- BOURAOUI Rahma
