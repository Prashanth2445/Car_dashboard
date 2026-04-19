# Car_dashboard

🚗 Car Dashboard System using CAN Protocol (PIC18F4580)
📌 Overview

This project implements a real-time car dashboard system using the PIC18F4580 microcontroller and CAN (Controller Area Network) protocol.

The system receives vehicle parameters from different nodes (ECUs) over CAN bus and displays them on a 16x2 CLCD. It also controls indicator LEDs with timer-based blinking to simulate real automotive behavior.

⚙️ Features
📟 Display of:
Speed
RPM
Gear Position
Indicator Status
🔁 Real-time CAN data reception
💡 Indicator LED control (Left / Right / Hazard)
⏱ Timer0 interrupt-based blinking mechanism
🧩 Modular code structure
🧠 System Architecture
CAN Module → Receives data from other ECUs
Message Handler → Processes received CAN messages
CLCD Driver → Displays data on screen
Timer Module → Controls blinking of indicators
Main Control Loop → Integrates all modules
🛠️ Technologies Used
Embedded C (XC8 Compiler)
MPLAB X IDE
PIC18F4580 Microcontroller
CAN Protocol
16x2 CLCD Display
📂 Project Structure
├── main.c                # Main application loop
├── can.c                # CAN communication driver
├── clcd.c               # LCD driver functions
├── message_handler.c    # CAN data processing
├── timer0.c             # Timer and blinking logic
├── msg_id.h             # Message ID definitions
🔄 Working
CAN module receives data (Speed, RPM, Gear, Indicator)
Data is passed to message handler
Based on message ID:
Data is decoded
Display updated on CLCD
LEDs controlled accordingly
Timer interrupt ensures periodic LED blinking
💡 Key Learnings
Understanding CAN protocol in automotive systems
Real-time data handling in embedded systems
Interrupt-driven programming
LCD interfacing and debugging
Modular firmware design
🚀 Future Improvements
Add fault detection system
Integrate sensors for real-time input
Upgrade to graphical display
Add wireless diagnostics
🙏 Acknowledgment

Special thanks to my mentor Saravanan Sowrirajan and Emertxe Information Technologies for guidance and support throughout this project.
