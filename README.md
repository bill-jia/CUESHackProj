# MedFriend
##The Problem

One study in the USA found that 75% of adults do not adhere to medication prescriptions. People forget. This costs an estimated $100 billion annually in the USA alone. Smart reminders to help people remember medication means better health, and a better economy. 

##The Solution

MedFriend is a smart device that uses Bluetooth Low Energy (BLE) technology to sense when a medication bottle is opened. Depending on user choice, it can send alerts when:

+ Medication hasn’t been opened by a certain time
+ A container with potentially dangerous contents is opened.

Users interact with MedFriend through a simple mobile app to track their medication bottles, set reminders, and set alerts. 

##Further Opportunities 

MedFriend can be extended to track medication bottles in multiple locations by using local routers gather BLE signals and transmit them via a mobile network. 

This could further allow:

+ Helping care for loved ones by ensuring they take medication as prescribed;
+ Helping physicians track patient adherence to prescriptions; and
+ Helping researchers conduct medical studies.

##Sensor Design

Throughout the project, three main sensor designs were experimented. The goal was to detect the opening of the bottle. In the end, the KISS (Keep it simple, stupid!) approach delivered the best performance. Taking the KISS approach to an extreme, two parallel bare metal wires were placed at along the cap of the bottle, in such a way that the user would create an electrical contact between them. The circuit set up was the same as with the graphite patterns. This method proved to be the most effective, outperforming the others investigated for consistency and reliability.

The sensor was connected to a Red Bear Labs BLE Nano (Nordic nRF51822 SoC) board.

##Software design
The front-end was written in Angular 1.4 wrapped in Cordova and the back-end was written in Rails 4.2 with a PostGRES database. The code for the microcontroller was written with C++ on the mbed and yotta platforms.

## Contributors
+ Luca Donini
+ Edgar Gu
+ Bill Jia
+ Duncan McNicholl
