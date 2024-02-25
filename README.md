# Ultrasonic Sensor-controlled Servo Motor for Distance Measurement
This Arduino sketch utilizes an ultrasonic sensor and a servo motor to measure distances in its surroundings. The code starts by defining the pins for the ultrasonic sensor's trigger and echo, as well as initializing a servo object for controlling the servo motor. In the setup function, pin modes are set accordingly, and the serial communication is initiated for debugging purposes.

The loop function then rotates the servo motor from 15 to 165 degrees in increments, measuring distances at each degree using the ultrasonic sensor. The calculated distance values are sent over the serial port along with corresponding servo angles. Subsequently, the servo rotates back from 165 to 15 degrees while continuing to measure distances.

A separate function, calculateDistance(), is defined to compute the distance based on the time taken for the ultrasonic pulse to travel and return. This information is then utilized to derive the distance in centimeters.

Overall, this code enables the servo motor to sweep across a range while collecting distance measurements, providing a simple yet effective setup for proximity sensing applications.





