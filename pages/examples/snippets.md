# Code Snippets

This is a small collection of base projects to get you started. The focus on specific functionality and are a nice base to start a project from.

## Installing a Project

To install a project you will need a [resin.io][resin] account with an
application set up ready to receive code. See the
[getting started][getting-started] and [deployment][deploy] guides for details
on how to do this.

To deploy a project simply clone it and push it to your application's `resin`
endpoint. E.g. for the [Text to Speech Converter project][text2speech]:-

```
git clone https://github.com/resin-io/text2speech.git
git remote add resin [endpoint]
git push resin master
```


### Resin-ssh

[Repository][resin-ssh]
[Repository][resin-ssh-node]

This basic resin project allows you to have local ssh access to your running container on your device. It does this by starting dropbear, a light weight ssh daemon, in a background process. There is both a node and a python demo of this, so you can get up and running fast. Please note, both of these have small webservers running in the main app, but these could be replaced by an infinite loop. This is needed because in order to ssh into a container, it has to have a long running process in it. That way docker does not close/destroy the container.

### Node.js and the RPI camera module
[Repository][picamera-node]

A basic skeleton application to get you up and running with the raspberry pi camera module using node.js

### Python and the RPI camera module
[Repository][picamera-py]

A basic skeleton application to get you up and running with the raspberry pi camera module using python.

### Analog-to-digital converter

[Repository][ADC_py] by [Shaun Mulligan][shaun-mulligan]

This is a simple project so show to read analog sensor values into the raspberry pi using python. It uses the [ADS1x15][ADC_adafruit] family of I2C analog-to-digital converters to read in analog signals between 0 and 3.3V.

### resin-tether

[Repository][resin-tether] by [petrosagg][petrosagg]

This python project allows you to share your ethernet connection to wifi. It essentially allows the raspberry pi to act as a wifi access point.

### Avahi Daemon on Raspberry Pi

[Repository][avahi-example]

This simple example demonstrates how to get the avahi daemon running on your resin.io device. From this example you will be able to access your device from `<RESIN_UUID>.local` on your local network. The `<RESIN_UUID>` is the ID shown on the resin.io device dashboard.

### Example GPIO control in node.js

[Repository][example-pi-pins]

A simple application which demonstrates the use of the [Pi Pins][pi-pins]
library to interface with [GPIO][gpio].

### Example GPIO control in python

[Repository][py-gpio]

A simple application that shows you how to toggle the general purpose I/O pins on the raspberry pi using python.

### Example servo motor control in node.js

[Repository][servo-motor-node] by [Craig Mulligan][craig-mulligan]

A simple application that shows you how to issue commands to a servo motor using pi-blaster.


<!-- ###Code Snippets Links -->

[py-gpio]:https://github.com/resin-io-projects/resin-rpi-gpio-sample-with-python
[picamera-node]:https://github.com/resin-io-projects/resin-rpi-nodejs-picamera.git
[picamera-py]:https://github.com/resin-io-projects/resin-rpi-python-picamera.git
[ADC_py]:https://github.com/resin-io-projects/resin-rpi-py-ADC.git
[resin-tether]:https://github.com/petrosagg/resin-tether
[example-pi-pins]:https://github.com/resin-io-projects/resin-rpi-nodejs-basic-gpio.git
[avahi-example]:https://github.com/resin-io-projects/avahi-example.git
[resin-ssh]:https://github.com/resin-io-projects/resin-ssh-python.git
[resin-ssh-node]:https://github.com/resin-io-projects/ssh-node
[text2speech]:https://github.com/resin-io/text2speech
[servo-motor-node]:https://github.com/craig-mulligan/resin-servo-node

<!-- ###Team Github name links -->

[shaun-mulligan]:https://github.com/shaunmulligan
[craig-mulligan]:https://github.com/craig-mulligan
[aleksis]:https://github.com/abresas/
[lifeeth]:https://bitbucket.org/lifeeth/
[alex]:https://github.com/alexandrosm
[petrosagg]:https://github.com/petrosagg
[nghiant2710]:https://github.com/nghiant2710

<!-- ###general -->
[deploy]:/pages/deployment/deployment.md
[getting-started]:/pages/installing/gettingStarted.md
[resin]:https://resin.io
