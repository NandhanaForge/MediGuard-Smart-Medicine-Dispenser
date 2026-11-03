# MediGuard – Smart Medicine Reminder and Dispenser

## Overview

MediGuard is an affordable, smart medicine reminder and automatic dispensing system designed to help elderly people and patients manage their medication schedules safely.

The system uses an ESP32 microcontroller, a Real-Time Clock (RTC), servo motors, an LCD display, and a buzzer to remind users when to take their medicines.

Unlike traditional reminder systems, MediGuard provides physical access control by opening only the designated medicine compartment at the scheduled time.

## Problem Statement

Many elderly people and patients forget to take medicines at the correct time. Traditional medicine boxes and mobile reminders cannot prevent wrong-time dosing, missed doses, or accidental double-dosing.

MediGuard addresses these problems through automated reminders and servo-controlled medicine compartments.

## Objectives

- To develop an automatic medicine reminder system.
- To provide scheduled medicine dispensing.
- To prevent wrong-time and accidental double dosing through compartment access control.
- To display medicine information using an LCD.
- To alert users through an audible buzzer.
- To provide an affordable and user-friendly healthcare solution.

## Components Used

| Component | Purpose |
|---|---|
| ESP32 | Main microcontroller |
| DS3231 RTC | Accurate timekeeping |
| 16x2 I2C LCD | Display information |
| SG90 Servo Motors | Open and close compartments |
| Active Buzzer | Audio alerts |
| Push Button | Manual override |
| 5V 2A Power Supply | Power source |
| 1000µF Capacitor | Voltage stabilization |
| Jumper Wires | Circuit connections |
| Plastic Medicine Box | Enclosure |

## Working Principle

1. The ESP32 initializes all connected components.
2. The DS3231 RTC provides the current time.
3. The ESP32 continuously compares the current time with the programmed medicine schedule.
4. When the scheduled time arrives, the buzzer produces an alert.
5. The LCD displays the medicine name and compartment number.
6. The corresponding servo motor opens the correct compartment.
7. Other compartments remain locked.
8. The compartment closes automatically after the configured time or when the user acknowledges the alert.

## Features

- Automatic medicine reminders.
- Time-based medicine dispensing.
- Servo-controlled compartment locking.
- LCD-based medicine information.
- Audible buzzer alerts.
- Manual override functionality.
- RTC-based timekeeping.
- Optional Wi-Fi time synchronization using NTP.
- Low-cost and compact design.

## Software and Technologies

- Arduino IDE
- Embedded C/C++
- ESP32
- I2C Communication
- RTC Programming
- Servo Motor Control

### Libraries Used

- Wire.h
- RTClib.h
- LiquidCrystal_I2C.h
- ESP32Servo.h

## Hardware Connections

| Component | ESP32 Pin |
|---|---|
| LCD SDA | GPIO 21 |
| LCD SCL | GPIO 22 |
| Servo 1 | GPIO 13 |
| Servo 2 | GPIO 14 |
| Servo 3 | GPIO 15 |
| Servo 4 | GPIO 16 |
| Buzzer | GPIO 12 |
| Push Button | GPIO 17 |

Note: Verify the actual pin assignments against your final uploaded source code before wiring.

## Expected Applications

- Elderly patient medication management.
- Home healthcare assistance.
- Patients managing multiple medicines.
- Assisted living facilities.
- Healthcare monitoring systems.

## Future Enhancements

- Mobile application integration.
- Caregiver notifications.
- Medicine intake history and dose logging.
- Voice-based reminders.
- Fingerprint or RFID authentication.
- Medicine level detection sensors.
- Cloud-based monitoring.

## Project Team

- Nandhana P
- Nirjanna T
- Nirmal Kumar S
- Ragesh M

## Institution

KPR Institute of Engineering and Technology  
Department of Electronics and Communication Engineering  
Coimbatore, Tamil Nadu.

## Project Status

Hardware assembly and prototype development are described in the project report. Check the source code and current implementation before claiming that every feature is fully operational.

## License

This project is intended for academic and educational purposes.
