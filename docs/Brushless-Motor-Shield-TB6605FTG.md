---
name: Brushless Motor Shield (TB6605FTG)
category: 
bzurl: 
oldwikiname: 
prodimagename: 
surveyurl: 
sku: 105030027
---

![](https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/105030027-preview-wiki.jpg)

The Brushless Motor Shield (TB6605FTG) is a brushless motor driver for Arduino compatible system. It supports 9V ~ 24V DC input and can continuously and continuously output large current to drive the brushless motor. With the onboard potentiometer, you can adjust the motor speed easily. This shield offers a variety of modes to choose from, you can use the four onboard switches to switch functions.  
  
With the onboard Grove I2C interface, you can work with other grove modules with this shield easily, for instance, you can use a [Grove - LCD RGB Backlight](Grove - LCD RGB Backlight) to display the Motor speed. 
 
We also released the [TB6605 BLDC Motor Kit for Arduino](https://www.seeedstudio.com/TB6605-BLDC-Motor-Kit-for-Arduino-p-4024.html), which is based on this shield and contains an LCD and a high-quality brushless motor to display the Motor speed.



<p style=":center"><a href="https://www.seeedstudio.com/BLDC-Motor-Shield-TB6605-p-4025.html" target="_blank"><img src="https://files.seeedstudio.com/wiki/Seeed-WiKi/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>



## Feature

- Wide input voltage range: 9V ~ 24V
- I2C interface
- Hardware adjustable speed control(On-board Potentiometer)
- Multiple modes available: CW/CWW, Brake/Normal, Sine wave/Square wave


## Specification

|Parameter|Value|
|---|---|
|Supply voltage|3.3V / 5V|
|DC Power Input|9V ~ 24V|
|Max Output Current|0.02A|
|Driving mode|Sine wave/Square wave|
|Motor Interface|Screw terminal|
|External Grove Interface|I2C|


## Hardware Overview

### Pinout

<div align="center">
<figure>
  <a href="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/pinout.jpg" target="_blank"><img src="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/pinout.jpg" alt="TB6605FTG Brushless Motor Shield pinout" title="Pinout diagram" />
  <figcaption><b>Figure 1</b>. <i>Pinout diagram</i></figcaption></a>
</figure>
</div>


### Screw terminal definition

|Brushless Motor Shield|Brushless Motor            |wire color |
|----------------------|---------------------------|-----------|
|5V                    |Logic power supply positive|Red        |
|GND                   |Logic power ground         |Black      |
|HU+                   |Hall sensor Phase U        |Orange     |
|HV+                   |Hall sensor Phase V        |Dark Green |
|HW+                   |Hall sensor Phase W        |Dark Blue  |
|U                     |Coil Phase U               |Yellow     |
|V                     |Coil Phase V               |Light Green|
|W                     |Coil Phase W               |Light Blue |

<div align="center"><b>Table 1.</b><i>Wiring Map</i></div>


!!!Tip
        The wiring color may be different if you are not using the 42BLF01 brushless motor, please connect according to the specific situation




## Getting Started


### Materials required

- [Brushless Motor Shield (TB6605FTG) x1](https://www.seeedstudio.com/BLDC-Motor-Shield-TB6605-p-4025.html)
- [Grove - LCD RGB Backlight x1](Grove - LCD RGB Backlight)
- [Arduino or Seeedunio x1](https://www.seeedstudio.com/Seeeduino-V4-2-p-2517.html)
- Brushless Motor x1


Or you can just use our [TB6605FTG Brushless Motor Kit for Arduino](https://www.seeedstudio.com/TB6605-BLDC-Motor-Kit-for-Arduino-p-4024.html), this kit contains Brushless Motor Shield, 42BLF01 brushless motor, and a Grove - LCD RGB Backlight.


### Hardware connection

- **Step 1.** Connect the Brushless Motor to the Screw terminal of the Brushless Motor Shield, please refer to the **Table 1.**

- **Step 2.** Connect the Grove - LCD RGB Backlight to the Grove I2C port on the Brushless Motor Shield.

- **Step 3.** Plug the Brushless Motor Shield into your Arduino or Seeeduino.

- **Step 4.** Power the shield with DC jack and power the Arduino via USB cable.


<div align="center">
<figure>
  <a href="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/connect.png" target="_blank"><img src="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/connect.png" alt="brushless dc motor wiring" title="Pinout diagram" />
  <figcaption><b>Figure 2</b>. <i>Hardware connection</i></figcaption></a>
</figure>
</div>


### Software

!!!Attention
        If this is the first time you work with Arduino, we strongly recommend you to see [Getting Started with Arduino](https://wiki.seeedstudio.com/Getting_Started_with_Arduino/) before the start.



- **Step 1.**  
Download the [BLDC Motor Shield (TB6605) lib](https://github.com/Seeed-Studio/BLDC_Motor_Shield_TB6605) Library from Github. 
Download the [Grove-LCD RGB Backlight Library](https://github.com/Seeed-Studio/Grove_LCD_RGB_Backlight/archive/master.zip) Library from Github. 

- **Step 2.** Refer to [How to install library](https://wiki.seeedstudio.com/How_to_install_Arduino_Library) to install library for Arduino. 

- **Step 3.** Restart the Arduino IDE. Open the example, you can open it via the path: **File --> Examples -->BLDC Motor Shield (TB6605)--> TB6605_demo**. 


<div align="center">
<figure>
  <a href="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/ARDUINO.jpg" target="_blank"><img src="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/img/ARDUINO.jpg" alt="brushless dc motor arduino" title="Pinout diagram" />
  <figcaption><b>Figure 3</b>. <i>Demo Path</i></figcaption></a>
</figure>
</div>


- **Step 4.** Upload the demo. If you do not know how to upload the code, please check [How to upload code](https://wiki.seeedstudio.com/Upload_Code/).


!!!Success
		If everything goes well, you can see the DC motor run and the LCD will show the speed. Now you can rotate the potentiometer to control the speed of the motor.  


## Schematic Online Viewer

<div class="altium-ecad-viewer" data-project-src="https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/res/Brushless%20Motor%20Shield%20(TB6605FTG)%20v1.01.zip" style="border-radius: 0px 0px 4px 4px; height: 500px; border-style: solid; border-width: 1px; border-color: rgb(241, 241, 241); overflow: hidden; max-width: 1280px; max-height: 700px; box-sizing: border-box;" />
</div>


## Resources

- **[Zip]** [BLDC Motor Shield (TB6605) Eagle Files](https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/res/Brushless%20Motor%20Shield%20(TB6605FTG)%20v1.01.zip)

- **[PDF]** [42BLF01 Brushless Motor-Specification](https://files.seeedstudio.com/wiki/BLDC-Motor-Shield-TB6605/res/42BLF01-Specification.pdf)




## Tech Support

Please do not hesitate to submit the issue into our [forum](https://forum.seeedstudio.com/).
    <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://files.seeedstudio.com/wiki/Wiki_Banner/new_product.jpg" /></a></p>