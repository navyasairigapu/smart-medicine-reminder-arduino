# 💊 Smart Medicine Reminder System

> An Arduino-based embedded system that helps users take medicines on time using RTC-based scheduling, LCD reminders, and buzzer alerts.

---

## 📖 Project Overview

The **Smart Medicine Reminder System** is an embedded systems project designed to assist users — particularly elderly patients — in maintaining consistent medication schedules. The system uses a **Real Time Clock (RTC) module** to keep accurate time and continuously compares the current time against pre-set medication schedules stored in the system. When a scheduled medication time is reached, the system triggers a **buzzer alert** and displays a **reminder message on an LCD screen**, ensuring the user is notified clearly and on time.

This project demonstrates practical embedded systems integration — combining real-time timekeeping, display interfacing, and audible alerting into a single assistive healthcare device.

---

## 📝 Abstract

Missing medication doses is a common issue, especially among elderly patients managing multiple prescriptions on different schedules. Manual reminders (written notes, verbal reminders from caregivers) are often inconsistent or unreliable. This project presents a **Smart Medicine Reminder System** built around an Arduino microcontroller and an RTC module. The RTC continuously maintains accurate real-world time, which is compared against pre-set medication schedules programmed into the system. When the current time matches a scheduled dose time, the system activates a buzzer and displays a clear reminder message on an LCD screen. This combination of audible and visual alerts ensures the reminder is noticeable even if the user is not looking directly at the device. The system demonstrates a low-cost, reliable, and easily understandable solution for improving medication adherence.

---

## ❗ Problem Statement

Medication non-adherence is a significant and common challenge, particularly for elderly individuals or patients on multiple medications:

- Manual reminder methods (notes, verbal reminders) are **inconsistent and easy to forget**
- Elderly patients may have **difficulty tracking multiple medication schedules** unaided
- Missed or delayed doses can **reduce treatment effectiveness** and, in some cases, pose health risks
- Caregivers are not always present at the exact time a dose is due

There is a clear need for an automated, low-cost, and reliable reminder system that does not depend on a caregiver being present at the right moment.

---

## 🎯 Objectives

- To design an Arduino-based system capable of maintaining accurate real-time tracking using an RTC module
- To implement logic that compares current time against pre-set medication schedules
- To generate a clear audible alert via a buzzer when a scheduled dose time is reached
- To display a visible reminder message on an LCD screen at the scheduled time
- To create an assistive, easy-to-use system suitable for elderly patients

---

## 🏗️ System Architecture

The system architecture connects a microcontroller (Arduino) as the central processing unit, interfaced with an RTC module for timekeeping and an LCD + buzzer for output alerts.

**Input Side:**
RTC Module → Arduino (continuous time read)

**Processing:**
Arduino compares current time (from RTC) against pre-set medication schedule

**Output Side (triggered when scheduled time is reached):**
Arduino → LCD Display (reminder message)
Arduino → Buzzer (audible alert)

A complete block-level breakdown of this architecture is provided in `BLOCK_DIAGRAM.md`.

---

## 🧩 Components Used

| Component | Function |
|---|---|
| Arduino Microcontroller | Central processing unit; runs the time-comparison logic and controls outputs |
| RTC (Real Time Clock) Module | Maintains accurate, continuous real-world time tracking |
| LCD Display | Displays the medication reminder message to the user |
| Buzzer | Generates an audible alert when a scheduled dose time is reached |
| Power Supply | Provides power to the Arduino and connected peripherals |

---

## ⚙️ Working Principle

1. **Time Tracking:** The RTC module continuously maintains and provides accurate real-world time to the Arduino
2. **Schedule Comparison:** The Arduino continuously compares the current time (from the RTC) against pre-set medication schedule times stored in the system
3. **Alert Triggering:** When the current time matches a scheduled dose time, the Arduino triggers the output devices
4. **Notification:** The buzzer sounds an audible alert, and the LCD simultaneously displays a clear reminder message
5. **Reset/Continue:** Once acknowledged or after the alert period, the system continues monitoring time for the next scheduled dose

---

## 📸 Result Photos

*Add photographs of the completed hardware setup and system in operation below.*

| Description | Image |
|---|---|
| Complete hardware setup (Arduino, RTC, LCD, buzzer wired together) | `results/hardware_setup.jpg` |
| LCD displaying the medication reminder message | `results/lcd_reminder_display.jpg` |
| System in operation during a scheduled alert (buzzer + LCD active) | `results/alert_in_action.jpg` |

> Place actual result images inside the `results/` folder using the filenames above (or update the table with your chosen filenames), so they render correctly when this README is viewed on GitHub.

---

## ✅ Advantages

- Provides consistent, automated medication reminders without requiring caregiver presence
- Combines audible and visual alerts, increasing the likelihood the reminder is noticed
- Low-cost and simple to build using widely available components
- Particularly beneficial for elderly patients managing multiple medication schedules
- Reduces the risk of missed or delayed doses

---

## 🌍 Applications

- Home healthcare assistance for elderly or chronically ill patients
- Hospital or care facility bedside reminder systems
- Personal medication management for individuals on multi-dose schedules
- Academic demonstration of embedded real-time scheduling systems

---

## 🔭 Future Scope

- Adding support for multiple medicine slots with individually configurable schedules
- Integrating a mobile app notification system via Bluetooth or WiFi (e.g., ESP32-based upgrade)
- Adding a missed-dose logging feature for caregiver review
- Incorporating a snooze/acknowledge button for user interaction with active alerts
- Expanding the display to show upcoming dose schedules, not just active alerts

---

## 🏁 Conclusion

The Smart Medicine Reminder System demonstrates a practical, low-cost embedded solution for improving medication adherence. By combining an RTC module for accurate timekeeping with LCD and buzzer-based alerting, the system reliably notifies users when it is time to take their medication — without requiring constant caregiver supervision. This project highlights the value of simple, well-integrated embedded systems in addressing real, everyday healthcare challenges, particularly for elderly patients managing regular medication schedules.

---

## 👤 Author

**Navya Shree Sairigapu**
B.Tech, Electronics & Communication Engineering
https://www.linkedin.com/in/navya-sairigapu-97723935a · navyasairigapu@gmail.com
