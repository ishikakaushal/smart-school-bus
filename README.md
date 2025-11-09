# smart-school-bus
# Smart School Bus – RFID Attendance & GSM Notification System

This project is a safety and attendance automation system designed for school buses.  
It uses **RFID + Arduino + GSM** to track student boarding/unboarding and send real-time SMS alerts to parents.

---

## ✅ Objective
To improve school bus safety by:
- Automatically recording when students board and leave the bus
- Notifying parents through SMS in real time
- Reducing manual attendance errors

---

## ✅ Features
- RFID-based student identification  
- Auto detection of boarding/unboarding  
- SMS alerts using GSM module  
- Real-time monitoring  
- Low-cost hardware solution

---

## ✅ Hardware Used
- Arduino UNO  
- RFID RC522  
- GSM SIM900A / SIM800L  
- Buzzer  
- LCD 16x2 (optional)  
- Jumper wires + 12V adapter

---

## ✅ Technologies Used
- **C/C++ (Arduino IDE)**
- **SPI communication**
- **GSM AT commands**
- **RFID UID matching**
- **Serial communication**

---

## ✅ Project Workflow
1. System starts  
2. RFID scanner waits for a card  
3. Student taps RFID card  
4. System reads UID  
5. UID is matched with database  
6. Determines *boarding* or *unboarding*  
7. Sends SMS to parent  
8. Logs the event  
9. Waits for next scan  

---

## ✅ Wiring Summary
- RC522 → Arduino via SPI  
- GSM module → Arduino via SoftwareSerial  
- Separate 12V power for GSM  

(Detailed wiring in docs/wiring_diagram.md)

---

## ✅ Code Overview
Main logic:
- Read RFID UID  
- Check student status  
- Call `sendSMS()` function  
- Print status on Serial Monitor  

Full code inside:  
`code/smart_school_bus.ino`

---

## ✅ Outcome
- Works as an accurate attendance + safety system  
- Low-cost implementation suitable for schools  
- Real-time parent communication improves security  

---

## ✅ Future Enhancements
- GPS tracking  
- Firebase/Cloud attendance dashboard  
- Mobile app for parents  
- Face recognition (optional)

---

## ✅ Author
**Ishika Kaushal**  
(Developer of the Smart School Bus automation system)
