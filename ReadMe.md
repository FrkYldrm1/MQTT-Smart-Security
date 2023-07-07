# MQTT Smart Security
*This is a group project made by Etka Kocak and Faruk Yildirim. The report is personal and the author of this report is Faruk Yildirim.*  

**Author: Faruk Yildirim (fy222av)**  
**Course: 1DT305 - Introduction to IoT**  

MQTT Smart security is a security system that can be used in a variaty of the places such as homes, work places, and businesses. The system will provide extra security for the environment that is set up. The system consists of two circuits. The first circuit is an alarm with a sensor that can be installed in any door. The second circuit is a device with multiple security sensors that will provide security to the environment that is installed. 

Approximate time required to replicate the project: **2-3 hours**

## Objective

Security is the main need for humanity since we exist. We build castles, homes, and fences to be more secure. The advancements in technology and our civilization brought new dangers that we face in daily life. For example gas leak. If we look back five hundred years ago humanity didn't have such a danger. The high buildings that we build now should be more secure against earthquakes. The main objective for me to pick this project is; to improve security with technology, against incidents that we cannot control. For example natural disasters like earthquakes or gas leaks. In today's world, we can minimize the deaths caused by this kind of incident. The sensors and the internet that we use can detect danger and inform people with notifications or information that is provided via security systems and help us to satisfy our need to feel safe.


Circuit 1 of the MQTT Smart security system has an ultrasonic distance sensor. These sensors can be found in automobile self-parking technology or in robotics. It measures the distance by using ultrasonic waves. This sensor is used to detect people or animals who enter the room. The system is installed on the doors. It uses MQTT to send notifications to your phone. It also sets the alarm and starts to light a red LED. The alarm can be controlled via phone.

Circuit 2 is more complex than the first circuit. Circuit 2 consists of four different sensors. There are also three LEDs. All four sensors use MQTT to send notifications to your phone.

**Flame Sensor**  
The flame sensor measures the intensity or heat to detect the fire. When the sensor detects the fire, it sends a notification to the phone. When the fire is under control you can reset the sensor via phone.

**Vibration Sensor**  
Natural disasters are the things that we cannot control. When an earthquake happens during your sleep you might not be able to act in time to find a safe place. The vibration sensor will inform you via notifications to your phone. In that way, the danger can be minimized.
**The Gas Sensor**  
Gas leaks are one of the reasons for deads in our age. Every year lots of people die because of gas leaks. The gas leak sensor will detect the leak and inform the user so the user can avoid danger.

**Temperature/Humidity Sensor**  
The temperature and humidity sensor is an additional feature that we added to this system. You can see detailed data about temperature and humidity in the environment. In that way, users will have more control over the environment.


Cost-effectiveness: The MQTT Smart security system is also cost-effective. This system is easy to build and the sensors that are used in the system are highly accessible so production of the system will be cheap and easy. Due to its cost-effectiveness, it can provide security for a wide range of users.

Easy installation and use: The other important thing with the system is, it is easy to install and use. The system only should be installed in an environment that is aimed at security. The ultrasonic wave sensor should be attached to the door and other sensors can be installed at any place in the room. Then users can get notifications through the MQTT dashboard app.

Remote monitoring and control: The system will provide remote control to the user via the internet. The user will be able to monitor and control the sensors through the mobile application.


## List of material
|Component |Function |Price and link |
|-|-|-|
|Raspberry Pi Pico W |Programmable microcontroller with WiFi |[98.00 SEK](https://www.electrokit.com/en/product/raspberry-pi-pico-w/) | 
|DHT11 digital temperature and humidity sensor |Sensor for measure humidity and temperature  | [49.00 SEK](https://www.electrokit.com/en/product/digital-temperature-and-humidity-sensor-dht11/) | 
|HC-SR04 ultrasonic distance sensor |Sensor for detecting the distance to an object using sonar | [59.00 SEK](https://www.electrokit.com/en/product/distance-sensor-ultrasound-hc-sr04-2-400cm/) | 
|Pcs Ir Flame Sensor Module |Sensor that can detect a fire or any other bright light sources | [120.49 SEK](https://www.amazon.se/flamsensor-flamdetekteringsmodul-flamdetekteringssensor-kompatibel-justerbar/dp/B095Q6BW85/ref=sr_1_20?crid=29QIEGVQM7K4J&keywords=Pcs+IR+Infrared+Flame+Sensor+Module&qid=1687994286&sprefix=pcs+ir+infrared+flame+sensor+module%2Caps%2C123&sr=8-20) | 
|SW-420 vibration sensor |High sensitivity non-directional vibration sensor | [3.31 SEK](https://www.aliexpress.com/item/32954150924.html?pdp_npi=2%40dis%21SEK%213%2C31kr%213%2C09kr%21%21%21%21%21%402103011116879947026103811ef6e3%2166297503897%21btf&_t=pvid:7e2cd612-34b9-488e-bc54-46d429f7d5d4&afTraceInfo=32954150924__pc__pcBridgePPC__xxxxxx__1687994702&spm=a2g0o.ppclist.product.mainProduct) | 
|MQ-2 gas sensor |Smoke and combustible gas sensor that can detect flammable gas in a range of 300 - 10000ppm | [11.35 SEK](https://www.aliexpress.com/item/1005002742237575.html?&_t=pvid:de58b1a8-b9d3-45bb-92d2-4b4a610e9e9e&afTraceInfo=1005002742237575__pc__pcBridgePPC__xxxxxx__1687994954&spm=a2g0o.ppclist.product.mainProduct) | 
|LED traffic lights light-emitting module |A device that collects LEDs of 3 different colors in a single module | [8.82 SEK](https://www.aliexpress.com/item/32891804932.html?pdp_npi=2%40dis%21SEK%218%2C82kr%217%2C16kr%21%21%21%21%21%402103010c16879951118826566e7bf9%2165741865597%21btf&_t=pvid:424926ad-fb26-412c-89da-0ed2ade8d03c&afTraceInfo=32891804932__pc__pcBridgePPC__xxxxxx__1687995112&spm=a2g0o.ppclist.product.mainProduct) | 
|Buzzer |Audio device that generates a sound from an incoming electrical signal | [37.50 SEK](electrokit.com/en/product/buzzer-3-8-khz/) | 
|LED red |Semiconductor, diode-based, light-emitting electronic circuit element | [9.00 SEK](https://www.electrokit.com/en/product/led-red-3-mm-low-current-2ma-tllr4401/) |   

## Computer Setup

* Raspberry Pi microcontroller is used in this project.  
 * Thonny IDE is used as software. 
 Due to its simplicity, Thonny IDE is chosen for this project.

You can follow the steps below if you choose it:

**1- Download**  
[Download Thonny IDE](https://thonny.org/)  

**2- Setup Raspberry Pi Pico W**  
![image](/img/setup1.png)  
The green arrow shows that you need to select the raspberry pi.
Both circuits have their own folders Circuit1 and Circuit2. These files separately need to be uploaded to separate microcontrollers in order to make the system work. We used two different microcontrollers for both circuits.

**3- Libraries**  
![image](/img/setup2.png) 

The libraries that are used in the code might be missing. The libraries that are used in this project can be found on Pico W devices that have been installed. You can download the missing libraries from tools as shown in the pictures. 

**4- WiFi**
In order to make the system work some parts of the code should be personalized. The SSID and password for the Wifi should be changed in the code. 
```/Circuit1/main.py```:
``` Python
wlan.connect("SSID HERE", "PASSWORD HERE") # line 38
```
```/Circuit2/main.py```:
``` Python
wlan.connect("SSID HERE", "PASSWORD HERE") # line 76
```

**5- MQTT**  
The MQTT cloud server account must be created in order to make the code run. If you already have an existing account you can choose it from [io.adafruit.com](io.adafruit.com).
When you have an existing account, the topics should be created in the feeds section with the names that are provided below. 
* Mykey ![image](/img/setup3.png)  

As it is shown in the image the topics should be created with the names that are provided from the feeds section. The personal key must be written which will be found in the My Key section.
 

```/Circuit1/main.py```:
``` Python
mqtt_server = "io.adafruit.com" # line 26
topic = "YOUR_USERNAME/feeds/sui" # line 28
user = "YOUR_USERNAME" # line 29
password = "YOUR_KEY" # line 30
```
```/Circuit2/main.py```:
``` Python
mqtt_server = "io.adafruit.com"  # line 16
user = "YOUR_USERNAME" # line 17
password = "YOUR_KEY" # line 18
topic_tem = "YOUR_USERNAME/feeds/tem" # line 20
topic_hum = "YOUR_USERNAME/feeds/hum" # line 21
topic_fire = "YOUR_USERNAME/feeds/fire" # line 22
topic_eq = "YOUR_USERNAME/feeds/eq" # line 23
topic_gas = "YOUR_USERNAME/feeds/gas" # line 24
```

**5- Mobile (optional)**  

Adafruit.com can also be used as a dashboard other than the cloud. The IoT data can be monitored by the personal computer. The MQTT Dashboard can be downloaded to your mobile phone and receive notifications via the application.

The Dashboard application that is used in this project is:
[Download Link](https://play.google.com/store/apps/details?id=com.app.vetru.mqttdashboard&hl=en_US)

**6- Run it**  

When you are done with making circuit connections, the system is ready to run. You can connect the system to an energy point(power bank, socket, or laptop) and run it.
  
## Putting everything together   

### Diagram of the Circuit 1:   
![image](/img/diagram_circuit1.png)   

### Diagram of the Circuit 2:   
![image](/img/diagram_circuit2.png)  

### Connections

The connections are shown in the diagram. The diagram explains GPIO connections also. Any change in the connections should be also changed in the code as well. The diagrams are created using by "Digital" design application. 

**Circuit 1:**  
* 1- ``Buzzer``: Consists of two pins (+)long and (-)short. The long pin (+) should be connected to GPIO and the short pin -(-) should be connected to a minimum 220Ω resistor. 

* 2-  ``LED``: Consists of two pins (+)long and (-)short.
The long pin (+) should be connected to GPIO and the short pin -(-) should be connected to a minimum 220Ω resistor.

* 3- ``HC-SR04``: Consists of the four pins; GND, Echo, Trigger and Vcc. The Vcc should be connected to the 3.3-volt output. The GND should be connected to GND. The Trigger should be connected to GPIO and Echo should be connected to other GPIO with a 1kΩ resistor and also should be connected to GND with a 1kΩ resistor.

**Circuit 2:**  
The Vcc pins should be connected to the 3.3-volt output and all GND pins should be connected to GND. No resistor is needed.

* 1- ``DHT11``:  Consists of three pins Vcc, Out, and GND. The Out pin should be connected to the GPIO without a resistor then it should be connected to the 3.3-volt output with a 4.7Ω resistor.
 
* 2- ``Flame``: Consists of three pins DO, GND, and Vcc. The DO  should be connected to the first GPIO and no resistor is needed then it should be connected to the 3. 10KΩ resistor and 3-volt output required.

* 3- ``SW420``: Consists of three pins DO, GND, and Vcc. The DO pin should be connected to GPIO and no resistor is required.
 
* 4- ``MQ2``: Consists of four pins Vcc, GND, DO, and AO. The DO pin will be connected to the GPIO and no resistor is needed. The AO pin is not required to be connected.

* 5- ``LEDS``: Consists of four pins G, Y, R, and GND. The G, Y, and R pins which are LEDs, should be connected to different GPIOs. There is no resister required.

## Platform  

The preferred cloud server is MQTT for this system. In that way communication between IoT devices is enabled. The MQTT allows the devices to communicate. It is a broker between the devices. 

Adafriuit.com is used as a cloud server platform and the MQTT Dashboard application is used as a dashboard. The MQTT Dashboard application allows me to receive notifications from my mobile device. 

## Transmitting the data/connectivity
* Used wireless protocol: **WiFi**  
* Used transport protocol: **MQTT**  


Circuit 1 sends the data when the alarm is triggered. The change of movement in the sensor will send a notification. The data is binary so when the alarm is triggered the data that will be sent is 1. The triggered alarm will send the data to the "sui" topic. If the user response with data 0 to the "sui" topic the alarm will turn off and wait for the new movement.

 Circuit 2 is also the same as Circuit 1. Detectors communicate with binary data 0 and 1. When the data is on the notification is sent to the user and the user can respond with 0 to close the alarm. The binary communication logic is not valid for the temperature and humidity sensors. This sensor sends data (celsius and percentage) every two seconds. No notification is required in this case because it is only one-way communication. The data is sent to "tem" and "hum" topics. The user can check the data from the dashboard application if it is needed.

## Presenting the data

### Dashboard
![image](/img/dashboard.jpg)

The image shows the UI of the MQTT Dashboard application. The alarm button communicates with the first circuit and when the alarm is triggered, it can be stopped with the alarm button. The other buttons that are presented in the image belong to the second circuit and alarms also can be controlled from the dashboard. The DHT11 is where the one-way communication happens and data about humidity and degree is presented.
  

### Database
The database is not accessible through the MQTT mobile app. It can be accessed through an Adafruit.com account. Data is saved in the database every three seconds for the temperature and humidity sensor and for the other four sensors data is saved when there is communication between the user and sensors. For example, if the fire alarm is triggered the database will save the alarm, and if the user responds the data also will be saved.

![image](/img/database_fire.png)
The image shows the database of the Fire Detector. The communication is can be seen in the image. The 1 refers to a fire alarm and the 0 means that the alarm is taken under control.


![image](/img/database_tem.png)

The image shows the database for the temperature. The chart shows the data about temperature within a time interval.

## Final result

### Circuit 2:
![image](/img/circuit2_1.jpg)
![image](/img/circuit2_2.jpg)

### Circuit 1:
![image](/img/circuit1_1.jpg)
![image](/img/circuit1_2.jpg)

### Final thoughts

The project is added a lot to me. I learned a lot about IoT and the project was the application of the knowledge. When I was done with the project I realized the things that can be done with circuits and sensors are unlimited. I feel more comfortable and confident now in understanding IoT devices. The amount of time I had and the result I get is really promising. If there would be more time I believe that the end result could be more advanced and complex. In summary, the system that is developed is way much better than I imagined and I am very happy with the result. 


