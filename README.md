# ChicksiIoT_v01
Equip a Campingcar with a remote acecess

## Project motivation and purpose 
	1) Explore benefits to retrofit a camping car with IoT
	2) Use as basis to consider a business (selling devices-services)
	3) Prevent damage from camping car (see use case freezing and stealing)

## USE Cases and User Stories
The former project was: Wio GPS Tracker Seed 
### Former use cases
Use Cases of Wio GPS project
	1) Car is parked in the winter: Temperature drops below freezing point which will destroy water piping system: Reasons can be defect heater or heater disconnected from 230V supply
	2) Camping Car is parked and thiefs are entering the car to steal it or/and steal interior
	3) GPS coordination are tracked during a trip as an addition to the chicksi tagebuch (logbook)

Use cases
	1) Refill fresh water tank 
	2) Replace butan gas tanks
	3) Pay the electrical bill - winter heating 
	4) Empty gray water tank
	5) Heat the camping car interior from remote
	6) Plan new trips based on the route of prior trips
	
Unique Selling points
	1) Allows actions so that the water piping in winter is not destroyed  when a power out occurs
	2) Can be retrofit to old camping cars 
	3) Does not need to add cables
	4) Provides intrusion alert
	5) Alarms in case of gas leakage even if you are not in the car
	6) Informs you about the power consumption 
	7) Creates automatically a GPS logbock - so you can see where you have been
	8) Start remote the heating
	

Customer Requirements
The System shall
	1) Alarm the user when the inner temperature drops below a defined value (5 degree Celsius)
	2) The Temperature Limit must be adjustable anytime
	3) Measure the interior temperature & humidity
	4) Measure the outside temperature & humidity
	5) Detect motion in the campingcar interior 
	6) Alarm the user when butane gas is detected in the camping car interior
	7) Store the measured values
	8) Visualise the stored values
	9) Inform the user about the system Status on request (Battery voltage, measured values)
	10) Inform the user about the fill level of the butane gas tanks
	11) Inform the user about the fill level of the fresh tank while the tank gets filled
	12) Log the GPS coordinate when the vehicle is mooving - 
	13) Display the logged GPS coordinates on a map, according to selected dates
	14) Remotly controlled illuminate the car interior
	15) Remotly start the heating of the  car (enabled by alde heating)
	16) Write variables of interest (Temperature, Intrusion alert, Powerloss, etc (see above) into a log file (in case the cloud connection failed)
	

Nice to have or Future Requirement : Add a OBDII Adapter to the car and read motor values, speed, etc

Non Functional Requirements
	1) The system shall indicate if connected to the cloud services
	2) The system shall enable debugging (Add display?)
	3) Test the power-loss function
	4) Test the alarming of the system
	5) Create an error and event Log- that can be analyzed later on
	6) 
	



MVP - Minimal viable Product
In general a MVP describes a Solution which offers a minimal acceptable value for the user. In this case the Function: Alarm the user when the power is cut and the interior temperature falls below 5 degree, is defined as MVP. Thus the User can takes action and inform the Parkinglot owner to repair the power supply.
The satellite boxes can be added in a later stage.

Requirements for the MVP
1) Measure the interior temperature & humidity
2) Measure the outside temperature
3) Alarm when power loss and temperature below 5*C using IFTT
