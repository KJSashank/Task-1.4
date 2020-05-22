# ESP8266 Clock
## Main Divisions
* Push button
* ESP 32
* LED display
* Code

## Troubleshooting
If the led display shows no display, check the power supply... if all wiring is correct then the led display is not working, you have to get a new one assuming there is no fault with the ESP.
If the led shows display, but the information is incorrect or if the pushing the button gives a faulty display, check these out:

### Code
This is the main part of the project so make sure everything is right in here, check the wifi ssid and password again.

### ESP 32
It is very less likely that the ESP is at fault as there are mechanisms to prevent it from frying, check if the IC is hot. If you have problem in putting code in it or it fails to respond, there should be a problem with it, but again its not likely so chceck if the problem is with one of the other components.

### LED display
Sometimes some LEDs may be damaged giving wrong info, so check for multiple values if the the same LEDS dont light up when they have to...if yes then you have to try to get it repaired but it takes the same cost as buying a new one but just a bit less, so if you dont like waiting too much and spend too much time to repair it, buy a new one.

### Push button
There is seldom chance that push button is faulty, so check with serial monitor if the push button is giving the required result, assuming the wires are properly connected to it, else just buy a new one it is inexpensive.

### Website
There is a chance that your circuit is completely correct and everything is functional but the NTP has a problem, i.e  pool.ntp.org does not give accurate info, but it is a universal global website so there is almost no chance of it being wrong unless the server is down, so check the above points again carefully... if the server is down you have to wait else you can try another globally accepted website to gain info as it has literally 0 chance of happening, im ommiting the alternative website. PS- you can try finding an alternative website:p

## Components
* ESP 32 - [Mouser ESP-32](https://robokits.co.in/iot-internet-of-things/esp32-development-board-wifi-bluetooth)
* LED display - [clock LED](https://www.indiamart.com/proddetail/4-digit-7-segment-display-module-for-arduino-tm1637-21664562773.html)
              [7 segment for city](https://www.indiamart.com/proddetail/seven-segment-display-20357853397.html)
* Push button - [Pushbutton](https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwjmr6vRvsfpAhWVrZYKHWWaDdYYABAFGgJ0bA&ohost=www.google.com&cid=CAESQeD2Y5nlCpDNKLRnX8xPldG1aTgu02Z1YENbyiKjhCu-Gdy1Rm4h3MCVbiFzE_dLHIM21nbarc0k-LhSKreFRnTW&sig=AOD64_0K8Aas0a_Lboj6j_EnBJJbovnUOQ&ctype=5&q=&ved=2ahUKEwiOj6LRvsfpAhWHxjgGHXMUCCAQ9aACegQIDxBQ&adurl=)
