
# 3.5 Inch Soil Moisture Sensor

<img src="img/Soil Sensor.jpg"
     alt="Soil Moisture Sensor"
     style="float: left; margin-right: 10px;" />


## Working
The Soil Moisture Sensor uses capacitance to measure dielectric permittivity of the surrounding medium. In soil, dielectric permittivity is a function of the water content. The sensor creates a voltage proportional to the dielectric permittivity, and therefore the water content of the soil. The sensor averages the water content over the entire length of the sensor. There is a 2 cm zone of influence with respect to the flat surface of the sensor, but it has little or no sensitivity at the extreme edges.The Soil Moisture Sensor is used to measure the loss of moisture over time due to evaporation and plant uptake,evaluate optimum soil moisture contents for various species of plants,monitor soil moisture content to control irrigation in greenhouses and enhance bottle biology experiments.

## Specification
- Working Voltage:5V
- Working Current:<20mA
- Interface type:Analog
- Working Temperature:10°C~30°C


```cpp

int sensorPin = A0;    // select the input pin for the potentiometer
int sensorValue = 0;  // variable to store the value coming from the sensor
void setup()
{
 Serial.begin(9600);  
}
void loop() 
{
 sensorValue = analogRead(sensorPin);  // read the value from the sensor:  
 delay(1000);          
 Serial.print("sensor = " );                       
 Serial.println(sensorValue);                   
}

```