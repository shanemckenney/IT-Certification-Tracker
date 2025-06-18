# IT-Certification-Tracker

Built using Google Sheets and Apps Script, this project provides streamlined tracking, visual reporting, calendar automation, and instructor tools for bootcamp environments like the Cyber Warrior Program (CWP).

## **Features**

- Interactive Dashboard
   - Live stats per certification (pass percentage, total passed, third attempt list)
   - Visual color-coded status blocks
   - Highlights students who have completed all certifications

- Calendar Integration
   - Automatically creates Google Calendar events from exam date/time cells
   - Events are scheduled for 90 minutes and include popup and email reminders
   - Skips events scheduled in the past

- Blackout Logic for "Pass"
   - When a student passes an attempt, remaining attempts for that certification are blacked out to prevent         accidental input
   - Provides clear visual feedback using formatting

- Per-Certification Sheet Generation
    - Automatically creates dedicated, trimmed, and well-formatted sheets for each certification (e.g., A+ Core       1, Network+, etc)
    - Preserves formatting from the main tracker
    - Limits display to the top 24 student rows for clarity

- Custom Instructor Menu
    - Adds a "CWP Tools" menu with options to:
        - Create Calendar Events
        - Blackout Passed Attempts
        - Build Exam-Specific Sheets

## Setup Instructions

- Make a copy of the sanitized template Google Sheet (link coming soon)
- Open Extensions > Apps Script
- Replace any existing code with the scripts found in the /scripts folder
- Run onOpen() once to activate the CWP Tools menu

- Use the custom menu to:
    - Generate per-certification sheets
    - Create calendar events based on scheduled exam entries
    - Apply blackout formatting based on passed attempts

## Screenshots



## FERPA Compliance

This repository contains only placeholder data (e.g., "Student 01") and no personally identifiable student information.

The included template sheet and screenshots are fully sanitized and safe for public sharing.

## Repository Structure

CWP-Certification-Tracker/
├── /screenshots
│   └── dashboard-preview.png
├── /scripts
│   ├── blackoutPassedAttempts.js
│   ├── createCalendarEvents.js
│   ├── buildFormattedExamSheets.js
│   └── onOpen.js
├── /template
│   └── [Google Sheet Link Here]
├── README.md
└── LICENSE

## Intended Audience

- IT certification instructors
- Career school training coordinators
- Academic support staff responsible for student certification pipelines

## Technical Overview

- Google Sheets
- Google Apps Script
- Google Calendar API (for event automation)

## License

MIT License
