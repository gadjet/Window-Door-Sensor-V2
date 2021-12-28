# Window-Door-Sensor-V2
This is the second version of the Window Door sensor transmitter PCB
It uses an ESP 12F and some extrnal logic gates to wake up the ESP from a deep sleep whenever the door is opened or closed.
In my software configuration I use the ESP NOW protocol to send a data packet whenever the ESP is woken up, which takes around 600mS and is received by another ESP that is permenantly powered up.  I have the receiver (WEMOS D1 Mini) connected to the serial port of a Raspberry Pi running Node Red, with Node Red I can direct the message to any number of messaging protocols like email, MQTT. Pushover, pushbullet, Telegram ........ the list goes on.
