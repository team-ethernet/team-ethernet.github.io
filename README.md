# The Team

We are a team of students studying Information and Communication Technology at KTH Royal Institute of Technology in Stockholm. 
We are currently taking the course [II1305 Project in Information and Communication Technology](https://www.kth.se/student/kurser/kurs/II1305), during which we are conducting a project.

## Internet of Noisy Things
We are developing a noise sensor network for [KTH Network Systems Lab](https://www.kth.se/cos/research/nslab).
The project goal is to design and implement a complete network of noise sensors including
- Input of data from noise sensors.
- Connecting noise sensors in a wireless sensor network.
- Storage and access of sensor data.
- Web interface for accessing and displaying sensor data.

We will also, time permitting
- Investigate server-side support for CoAP pubsub.
- Investigate alternative solutions for noise measurements.

## How the project went

Our first goal was to gather noise data from a network of noise sensors and display the data on a website.
Our second goal was to implement support for sending the noise data messages in CBOR format through an API. This goal was added in the middle of the project as we succeeded with the first goal.

### Microphone

We used the Sen0232 noise sensor microphone connected to an MCU. The sensor outputs a voltage that is proportional to the sound level. We then convert the voltage to dB.

### SenML & CBOR API

Our sensors send their data in a standard called SenML (Sensor Measurement Lists). Anyone that uses our SenML API can easily send sensor data in both JSON and CBOR format. CBOR is more compact, saving memory and power.

### Front end & Back end

The noise data is visualized as graphs on our website. Thanks to our API you can specify what data you want to see. You can set a time interval, dB-interval, etc. You can also download the data. We even added the feature to live-update the graphs. 

## Guides and reports

These are the guides and reports we produced during the project.  

### Guides

+ [Front end development.pdf](guides\Front end development.pdf)
+ [Getting started with the database and backend.pdf](guides/Getting started with the database and backend.pdf)
+ [How to install and use Mosquitto for Windows.pdf](guides\How to install and use Mosquitto for Windows.pdf)
+ [Instructions for setting up toolchain for microcomputer.pdf](guides\Instructions for setting up toolchain for microcomputer.pdf)
+ [Running simulated sensors with simsens.jar.pdf](guides\Running simulated sensors with simsens.jar.pdf)

### Reports

+ [Noise sensor diagnostic evaluation 1.0 2019-05-21.pdf](reports\Noise sensor diagnostic evaluation 1.0 2019-05-21.pdf)
+ [Sen0232 analysis 1.0 2019-05-21.pdf](reports\Sen0232 analysis 1.0 2019-05-21.pdf)
+ [SenML API encode CBOR evalutation 1.0 2019-05-20.pdf](reports\SenML API encode CBOR evalutation 1.0 2019-05-20.pdf)

## Team members
Anton Bothin abothin@kth.se  
Erik Flink erikfli@kth.se  
Nelly Friman nellyf@kth.se (Internal product owner)  
Jacob Klasmark jacobkl@kth.se  
Valter Lundegårdh valterlu@kth.se (Scrum Master)  
Isak Olsson isakol@kth.se  
Andreas Sjödin ansjod@kth.se  
Carina Wickström carinawi@kth.se  

If you have questions about the project, please contact our Scrum Master Valter Lundegårdh.

# Sprint 1: 23-29 April
Sprint Goal:
  - Design System & Prepare for development 

Sprint backlog (Estimates in paranthesis):
  - Linux + Toolchain (13)
  - Data design (8)
  - Database design (13)
  - Web page design (20)
  - Complete system design (8)
  
Estimated velocity (52)

Schedule:
  - Sprint Period: 2019.04.23-2019.04.29
  - Daily Scrum: 8:15 in 304
  - Sprint demo: 2019.04.29, 08:00 in Sal-B

# Flow-chart

[![Flow-chart](images/Back end.png "Flow-chart")](images/Back end.png)

# Sprint 2: 2-8 May
Sprint Goal:
  - SenML + CBOR Support 

Sprint backlog (Estimates in paranthesis):
  - SenML messages (13)
  - CBOR on sensors (40)
  - CBOR on server (8)
  - Design SenML API (8)
  - Implement SenML API (100)
  - Frontend API access (40)
  
Estimated velocity (209)

Schedule:
  - Sprint Period: 2019.05.02-2019.05.08
  - Daily Scrum: 8:15 in 304
  - Sprint demo: 2019.05.08, 08:00 in Sal-A


# Sprint 3: 9-15 May
Sprint goal: 
  - Finish SenML API and implement new front end feature.

Sprint backlog (Estimates in paranthesis):

## From Sprint 2 (20)
  - Tests for API 
  - Design senML API 
  - New microphone 
  - Implement senML API
  
## Sprint 3
  - Design senML decode API (20)
  - Look over documentation   (40)
  - Implment senML decode API on server (40)
  - Improve front end (13)
  - Live visualisation update (8)

Estimated velocity (240)

# Sprint 4: 16-22 May
Sprint goal: 
  - Finish implementing the API:s, clean up code, and prepare for the expo. 

Sprint backlog (Estimates in paranthesis):
  - Implement SenML decode API on server (40)
  - Implement SenML decode API on sensor (100)
  - Look over documentation   (40)
  - Evaluate CBOR (13)
  - Sliding window live update (5)
  - Implment senML decode API on server (40)
  - Code cleanup (8)
  - Github cleanup (8)
  
Estimated velocity (249)

Schedule:
  - Sprint Period: 2019.05.16-2019.05.22
  - Daily Scrum: 8:15 in 304
  - Sprint demo: 2019.05.08, 08:00 location TBA
