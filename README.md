# Grove Colour sensor driver for Mbed.js

To install, run in your mbed-js gulp based project:

```
$ npm install mbed-js-grove-colour-sensor
```

## Usage

```js
var color = GroveColourSensor(I2C_SDA, I2C_SCL);
color.powerUp();

setInterval(function() {
   print('R=' + color.readColour(GroveColourSensor.RED) + ', G=' + color.readColour(GroveColourSensor.GREEN) + ', B=' + color.readColour(GroveColourSensor.BLUE));
}, 1000);

