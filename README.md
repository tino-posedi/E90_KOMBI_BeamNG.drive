# BMW E90 instrument cluster CAN-Bus project

The BMW E90 instrument cluster project aims to interface and control the instrument cluster from a BMW E90 using a CAN-Bus Shield and an Arduino Uno. This project enables the gathering of information from the BeamNG.drive simulator and replicating the functionality on the physical instrument cluster.

## The idea behind this project
Modern vehicles utilize CAN (Controller Area Network) bus communication to interconnect various electronic control units (ECUs) within the vehicle. The BMW E90 instrument cluster project focuses on interfacing with the instrument cluster of a BMW E90 using a CAN-Bus Shield and an Arduino Uno. By interfacing the cluster with the Arduino and simulating CAN messages, the project aims to display data obtained from the BeamNG.drive simulator on the actual instrument cluster.

## Components
**To get started with this project, you will need the following components:**

- Arduino Uno
- CAN-Bus Shield (Seeed Studio or compatible)
- Jumper wires
- BMW E90 instrument cluster
- Power supply (12V 2.5A)
- USB Cable (for Arduino Uno)

## Software Tools
**The software tools used in this project include:**

- Arduino IDE for programming the Arduino Uno
- Visual Studio Code
- Spyder IDE

## Establishing connection to instrument cluster
**In this section I am going to describe how to connect instrument cluster to Arduino:**

- Connect Pin 6 to CAN-H (use male to female jumper wire)
- Connect Pin 7 to CAN-L (use male to female jumper wire)
- Connect Pin 9 to 12V (use laboratory power supply if possible)
- Connect Pin 18 to GND

CAN-H and CAN-L wires should be twisted tightly together to ensure that electromagnetic interference affects the signal in both wires uniformly. Connect CAN-H and CAN-L to CAN-Bus Shield (left CAN-H, right CAN-L).

Upload test sketch to Arduino Uno (included in this branch). Needles on your instrument cluster should sweep and come back to initial position.

## Troubleshooting
**There are few things that you should check if your instrument cluster is not behaving as it should:**

- Cut P1 line on the backside of your CAN-Bus Shield
- Baudrate for this type of instrument cluster should be 100KBPS

## Contributing
Contributions to this project are welcome! If you have ideas for improvements or want to add new features, feel free to fork this repository, make your changes, and submit a pull request.

## License
**This project is licensed under the MIT License.**
