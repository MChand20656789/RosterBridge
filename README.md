# RosterBridge
### Two-Job Scheduling & Shift-Conflict Detection Application

RosterBridge is a browser-based scheduling application designed for individuals managing multiple jobs with different work schedules. It provides a centralized weekly calendar to organize shifts, monitor working hours, estimate earnings, and identify scheduling conflicts.

The application helps users evaluate how shifts from two different scheduling sources fit together while accounting for overlapping work hours, overnight shifts, rest periods, and commute time.

## Features

- **Weekly Calendar:** View a seven-day schedule with previous-week, next-week, and current-week navigation.
- **Shift Management:** Create and delete shifts with customizable job names, dates, start and end times, locations, and hourly pay rates.
- **Multiple Job Sources:** Organize shifts from two scheduling sources: UKG Pro and Shift App.
- **Conflict Detection:** Identify overlapping shifts using time-interval comparisons.
- **Overnight Shift Support:** Calculate shift durations when an end time falls on the following calendar day.
- **Rest-Period Monitoring:** Configure minimum rest periods between shifts and identify schedules that do not satisfy the selected interval.
- **Commute-Time Allowance:** Account for configurable commute time when evaluating schedules.
- **Weekly Statistics:** Calculate scheduled hours, estimated gross pay, shift count, and overall schedule status.
- **Open-Shift Previews:** Evaluate sample open shifts against an existing schedule without adding them to saved shifts.
- **Data Persistence:** Store scheduling information and theme preferences in browser localStorage.
- **CSV Export:** Export scheduled shifts for external review and recordkeeping.
- **Dark and Light Themes:** Switch between display themes.
- **Responsive Interface:** Use the application across desktop and smaller screen sizes.

## Technologies

- HTML5
- CSS3
- JavaScript
- Browser localStorage
- CSV generation and export

## Technical Implementation

RosterBridge uses JavaScript to manage scheduling data, update the calendar interface, and perform time-based calculations.

Shift intervals are evaluated to identify overlapping schedules. Overnight shifts are handled by accounting for end times that fall on the next calendar day. Configurable rest-period and commute-time settings provide additional constraints for evaluating schedules across multiple jobs.

The application uses browser localStorage to retain scheduling information between sessions, while CSV export provides a way to retrieve and review saved shift data outside the application.

## Getting Started

No additional software installation or backend configuration is required.

1. Clone or download this repository.
2. Open `rosterbridge.html` in a web browser.
3. Create shifts for each job.
4. Configure your preferred rest-period and commute-time settings.
5. Review your weekly schedule, estimated earnings, and scheduling warnings.

## Project Structure

The current prototype is implemented in a single HTML file containing the application's HTML, CSS, and JavaScript.

```text
RosterBridge/
└── rosterbridge.html
```

## Current Limitations

RosterBridge is an independent browser-based prototype.

- Scheduling data is stored locally in the browser and is not synchronized across devices.
- UKG Pro and Shift App are represented as scheduling sources; the application does not directly connect to either platform.
- Open-shift previews are sample entries and do not support accepting or rejecting actual employer shifts.
- The application does not currently include user accounts, a remote database, or cloud synchronization.

## Project Purpose

This project explores practical software engineering concepts through a scheduling application, including time-interval algorithms, input validation, browser-based data persistence, dynamic interface rendering, and handling scheduling constraints.

RosterBridge demonstrates the application of programming and computational problem-solving to a real-world scheduling challenge.
