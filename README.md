# Temperature-Humidity-system-based-in-MQTT-Protocol
![publish temp με leds ](https://github.com/user-attachments/assets/43060f08-caab-4818-852a-76481909f255)

# Procedure for temperature and humidity measurements 
This procedure describes the steps by which you perform a measurement for temperature, humidity with the sht31 sensor via the ARM mbed simulator platform.More specifically, the transmission of data based on the MQTT communication protocol in cooperation with the MQTTBox application where we will be able to see the values we sent.

# Mbed Simulator by ARM
![Εικόνα1](https://github.com/user-attachments/assets/ca5a8fef-205d-45aa-888b-fd7ff3cf86b6)

Initially, Mbed is a platform and operating system for internet-connected devices based on 32-bit ARM Cortex-M microcontrollers. Such devices are also known as Internet of Things devices. There are several hardware demonstration boards for the Mbed platform, the first being the original Mbed microcontroller board. The Mbed microcontroller board (marketed as "mbed NXP LPC1768") is a demonstration board based on an NXP microcontroller, which features an ARM Cortex M3 core running at 96 MHz, with 512 KB of flash, 32 KB of RAM, and various interfaces, including Ethernet, USB Device, CAN, SPI, I2C, and other I/O.

# MQTTBox
![mqttbox τιμες ](https://github.com/user-attachments/assets/b88f1c82-4724-4afe-ad81-d1530c8ce948)

Developer utility for creating, developing and testing the MQTT connectivity protocol. MQTTBox allows us to create MQTT clients to publish or subscribe to topics, create MQTT virtual devices, test MQTT devices or brokers and much more.
MQTTbox has two formats:
* The add-on in the chrome browser.
* The nodejs App.

MQTTBox is a tool for developers that makes monitoring the MQTT Server a breeze. We can subscribe(subscribe) and publish(publish) topics using MQTTBox, as well as create a virtual MQTT device for testing and debugging. The best part is that we can use the same server for multiple purposes to make the most of our development workflow.

# PROJECT 
As I mentioned above in this demo we will see a simulation on the MQTT communication protocol based on the online platform of mbed Simulator. More specifically, 2 mqtt functions will be implemented to implement the program, the first one will have to do with the publish function in which by integrating component,the temperature - humidity sensor sht31 we will send the values of the sensor to the MqttBox application, where and which will help us at all the run time of the program to see the temperature values , humidity and even some other information like qos(Quality of Service), retain(Publisher can tell the broker to keep the last message in this topic), cmd-command(shows us the type of operation being performed), dup-duplicate(indicates that the message is duplicate and was sent again because the intended recipient did not acknowledge the original message. ),topic(a filter used by the broker in MQTT message deliveries), messageld(shows us the id of the message), lenght(the length of the message) and raw payload(the raw payload) by the time frame we have specified. But in addition we have also declared 2 leds, a red one for temperature and a blue one for humidity which will turn on and off depending on the limit we have set.
