# Calibrated-Distance-Counter using an Arduino and VL53L0X (LIDAR)
Here's the sensor from Adafruit: https://www.adafruit.com/product/3317

This library needs to be installed before you can use the sketch: https://github.com/pololu/vl53l0x-arduino



![ScreenShot](https://i.imgur.com/xPzf11u.png)

When the program starts, open a serial monitor of your choice (the standard Arduino IDE monitor is fine). A count down begins while the device is measuring distance. Whatever measurement the device is reading when the countdown reaches 0 is now the "calibrated distance". From this point on if anything is closer to the sensor than the calibrated distance, the "rep" (repetition) count will increment by 1.
