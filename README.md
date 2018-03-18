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
   print('R=' + color.readColour(GroveColours.RED) + ', G=' + color.readColour(GroveColours.GREEN) + ', B=' + color.readColour(GroveColours.BLUE));
}, 1000);

