# IT Certification Tracker for Instructors  
A Google Sheets + Apps Script Solution

This project was developed during my time as an instructor and mentor in the **Cyber Warrior Program (CWP)** at [MyComputerCareer](https://www.mycomputercareer.edu) — a career-focused technical training institution that equips students with both the certifications *and the real-world skills* needed to succeed in IT and cybersecurity roles.

The CWP is not a typical bootcamp. It’s a structured, immersive training experience built to prepare students for real-world challenges, not just exams. Students pursue certifications such as **CompTIA A+, Network+, Security+, and CySA+** while developing the practical knowledge needed to apply those skills in live environments.

---

## About This Project

This tracker was built to address the growing challenges of managing certification attempts, reporting metrics, and supporting student success across multiple exams and cohorts. While it started from a helpful base sheet shared by a fellow instructor (shoutout to Desmond), it quickly evolved into a full solution that saves **10+ hours per course cycle**, reduces errors, and improves student oversight.

### Pain Points Addressed:
- High risk of human error from manually tracking exam attempts and outcomes  
- No centralized agenda view to monitor exam days or know when to expect student results  
- Manual reporting burdens, especially when sharing updates with school leadership  
- Lack of clean metrics to track performance across students, certifications, and attempts

### The Solution:
Using **Google Sheets and Google Apps Script**, I engineered a system that:
- Automates data tracking and formatting across 5 certifications and 3 attempts per student
- Builds real-time dashboards for pass rates, completions, and third-attempt alerts
- Offers one-click calendar event creation, ensuring exam days are visible on Google Calendar
- Generates per-certification student sheets for focused analysis and administrative sharing
- Integrates a custom "CWP Tools" menu for instructors to manage everything in a few clicks

This solution has been fully sanitized and made FERPA-compliant for public use. It’s designed to be immediately useful for any career training program that tracks multiple certification pathways.

---

## Features

### Interactive Dashboard
- Live stats per certification (pass %, total passes, 3rd attempt alerts)
- Color-coded status indicators
- Highlights students who’ve completed all certifications

### Calendar Integration
- Automatically creates Google Calendar events based on sheet entries
- 90-minute events with email and popup reminders
- Ignores past dates to prevent clutter

### Blackout Logic for Passed Exams
- Automatically grays out remaining attempts after a pass
- Prevents accidental overwrites and improves data reliability

### Per-Certification Sheet Generation
- One-click export of trimmed sheets for each cert (A+, Net+, etc.)
- Retains formatting from master sheet

### Custom Instructor Menu
Adds a “Instructor Tools” menu with:
- Blackout Passed Attempts  
- Create Calendar Events  
- Build Per-Certification Sheets  

---

## Setup Instructions

1. Make a copy of the sanitized Google Sheets template (https://docs.google.com/spreadsheets/d/1QS6Ucy7CCDLJIYxjANq0xlJB4V3htEIIspRqs7RXcA0/edit?usp=sharing)  
2. Open **Extensions > Apps Script**  
3. Replace any code with the scripts from the `/scripts` folder  
4. Run the `onOpen()` function once to activate the custom menu  
5. Use the “CWP Tools” menu for automations and tracking

---

## Screenshots

![Dashboard Preview](screenshots/Dashboard.png)
![Dashboard Preview](screenshots/Instructor-Tools-Menu.png)
![Dashboard Preview](screenshots/Sheet-Layout.png)


---

## FERPA Compliance

This repository includes no real student data.  
- Student names have been replaced with placeholders  
- All screenshots and templates are fully sanitized  
- Safe for public use and academic sharing

---

## Repository Structure

