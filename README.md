https://iammoubee.github.io/software-engineering-and-project-management-project/




# Medique — Smart Clinic Appointment & Queue Management System

A web-based smart clinic appointment and queue management system designed to reduce patient waiting time, simplify appointment booking, and improve daily clinic workflow.

**Capstone Project — Department of ICT**  
**Session:** 2023–24  
**Student:** Sadia Kabir Mou  
**Student ID:** IT24016  
**Department:** ICT  

---

## Overview

**Medique** is a smart clinic appointment and queue management system that digitizes the patient journey from doctor selection to appointment booking and queue tracking.

The system provides separate interfaces for:

- **Patients** — Search doctors, book appointments, receive tokens, and track queues.
- **Doctors** — Manage schedules, view appointments, and control patient queues.
- **Admins** — Manage clinic operations, users, departments, appointments, and reports.

The current project is a **front-end prototype** developed using HTML5, CSS3, and JavaScript with realistic mock data.

---

## Problem Statement

Traditional clinic appointment systems often depend on:

- Manual registration and appointment booking
- Paper-based token systems
- Long and unpredictable waiting times
- Lack of real-time queue information
- Scheduling conflicts and double bookings
- High administrative workload
- Limited clinic performance data

Medique aims to address these problems through a simple digital appointment and queue management solution.

---

## Objectives

The main objectives of Medique are:

1. Develop a professional web-based clinic management prototype.
2. Allow patients to search and select doctors.
3. Enable online appointment booking.
4. Generate unique appointment tokens.
5. Provide live queue position and estimated waiting time.
6. Allow doctors to control their daily queues.
7. Provide administrators with management and reporting tools.
8. Demonstrate Object-Oriented design through UML documentation.
9. Provide a complete appointment-to-queue workflow.

---

## Key Features

### Patient Portal

- Patient registration and login
- Search doctors
- Filter doctors by specialization
- View doctor profiles
- View doctor schedules
- Book appointments
- Receive appointment token
- Track queue position
- View estimated waiting time
- Cancel appointments
- View appointment history
- Receive notifications

### Doctor Portal

- Doctor dashboard
- View today's appointments
- View current queue
- Call next patient
- Mark patient as served
- Skip patient
- Manage doctor schedule
- View appointment history

### Admin Dashboard

- Dashboard statistics
- Manage patients
- Manage doctors
- Manage departments
- Manage appointments
- Manage schedules
- Monitor queues
- Publish announcements
- View clinic statistics and reports

---

## Smart Queue System

One of the main features of Medique is the **token-based smart queue system**.

After successfully booking an appointment, the patient receives a unique token such as:

```text
A-27
```

The queue tracker displays:

- Current token
- Patient's token
- Patients ahead
- Estimated waiting time
- Queue status

The estimated waiting time is calculated using:

```text
Estimated Wait =
Patients Ahead × Average Consultation Time
```

This helps patients understand approximately how long they may need to wait.

---

## System Workflow

```text
Patient
   ↓
Search Doctor
   ↓
Select Doctor
   ↓
Select Date
   ↓
Select Time Slot
   ↓
Confirm Appointment
   ↓
Generate Token
   ↓
Join Queue
   ↓
Track Queue
   ↓
Doctor Calls Patient
   ↓
Consultation
   ↓
Mark as Served
```

---

## Project Architecture

Medique follows a **three-tier architecture**.

```text
┌─────────────────────────────────────┐
│       Presentation Layer            │
│     HTML5 + CSS3 + JavaScript       │
│                                     │
│ Patient | Doctor | Admin Portals    │
└─────────────────────────────────────┘
                  ↓
┌─────────────────────────────────────┐
│        Business Logic Layer         │
│                                     │
│ Appointments | Queue | Auth         │
│ Schedules | Notifications           │
└─────────────────────────────────────┘
                  ↓
┌─────────────────────────────────────┐
│             Data Layer              │
│                                     │
│ Users | Appointments | Queues       │
│ Schedules | Departments             │
└─────────────────────────────────────┘
```

The current prototype uses mock data. A real backend and database are planned for the full version.

---

## Object-Oriented Design

The system is designed around the following core classes:

```text
User
Patient
Doctor
Admin
Appointment
Queue
DoctorSchedule
Notification
Department
Clinic
```

### Main Relationships

```text
User
 ├── Patient
 ├── Doctor
 └── Admin

Patient
 └── Appointment

Doctor
 ├── Appointment
 └── DoctorSchedule

Appointment
 └── Queue

Patient
 └── Notification

Clinic
 └── Department
```

---

## UML & System Documentation

The project includes complete system design documentation:

- Context Level DFD
- Level-1 DFD
- Use Case Diagram
- Activity Diagram
- Entity Relationship Diagram
- Class Diagram
- Object Diagram
- System Architecture
- Gantt Chart

These diagrams describe the system's structure, workflow, database relationships, and object-oriented design.

---

## Prototype Screens

The prototype includes the following major screens:

| # | Screen | Description |
|---|---|---|
| 1 | Landing Page | Introduction and main navigation |
| 2 | Login / Registration | User authentication interface |
| 3 | Patient Dashboard | Appointment and queue overview |
| 4 | Find Doctor | Search and filter doctors |
| 5 | Doctor Profile | Doctor information and availability |
| 6 | Appointment Booking | Doctor, date, and time selection |
| 7 | Queue Tracking | Token and waiting-time tracking |
| 8 | Appointment History | Previous appointment records |
| 9 | Doctor Dashboard | Queue management interface |
| 10 | Admin Dashboard | Clinic management and statistics |

---

## Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Semantic structure |
| CSS3 | Styling and responsive UI |
| JavaScript ES6 | Front-end logic and interactions |
| Font Awesome 6 | Icons |
| Google Fonts — Inter | Typography |
| Git | Version control |
| GitHub | Source code hosting |
| LaTeX + TikZ | Documentation and diagrams |

---

## Current Project Status

### Current Version

**Front-end Prototype**

Implemented:

- Responsive user interface
- Patient flow
- Doctor search
- Doctor profile
- Appointment booking flow
- Token generation
- Queue tracking simulation
- Patient dashboard
- Doctor dashboard
- Admin dashboard
- Mock data
- UI interactions

### Not Yet Implemented

The following features are planned for the full system:

- Real backend server
- Real database
- User authentication
- Real-time queue synchronization
- SMS/email notifications
- Online payments
- Telemedicine
- Digital prescriptions

---

## Project Structure

A suggested project structure is:

```text
Medique/
│
├── index.html
├── README.md
│
├── css/
│   └── style.css
│
├── js/
│   ├── script.js
│   └── data.js
│
├── pages/
│   ├── login.html
│   ├── register.html
│   ├── patient-dashboard.html
│   ├── doctors.html
│   ├── doctor-profile.html
│   ├── appointment.html
│   ├── queue.html
│   ├── history.html
│   ├── doctor-dashboard.html
│   └── admin-dashboard.html
│
├── assets/
│   ├── images/
│   └── icons/
│
└── docs/
    ├── proposal.pdf
    ├── uml/
    └── dfd/
```

*Adjust the folder names above if your actual GitHub repository uses a different structure.*

---

## How to Run

Since the current version is a front-end prototype, no backend installation is required.

### Option 1 — Open Directly

Clone the repository:

```bash
git clone https://github.com/iammoubee/software-engineering-and-project-management-project.git
```

Go to the project directory:

```bash
cd software-engineering-and-project-management-project
```

Then open:

```text
index.html
```

in a web browser.

### Option 2 — VS Code Live Server

1. Open the project in VS Code.
2. Install the **Live Server** extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.

---

## Future Enhancements

The full version of Medique may include:

- Real-time queue updates using WebSockets
- SMS appointment reminders
- Email notifications
- Online consultation payment
- Telemedicine/video consultation
- Digital prescription management
- AI-based doctor recommendation
- Emergency appointment prioritization
- Native Android/iOS applications
- Multi-clinic support
- Real database integration
- Advanced clinic analytics

---

## Planned Full-Stack Technology

For future development, the system can be extended using:

```text
Frontend
HTML / CSS / JavaScript
        ↓
Backend
Node.js + Express
        ↓
Database
PostgreSQL
        ↓
Authentication
JWT
        ↓
Real-Time Queue
Socket.io
```

An alternative backend implementation can also be developed using **Django**.

---

## Software Process Model

The project follows an **Iterative and Incremental Software Process Model**.

### Iterations

**Iteration 1**
- Requirements gathering
- Literature review
- System design
- UML documentation
- Proposal
- UI mockups

**Iteration 2**
- Landing page
- Authentication UI
- Doctor search
- Doctor profile
- Appointment booking

**Iteration 3**
- Queue tracking
- Patient dashboard
- Doctor dashboard
- Admin dashboard

**Iteration 4**
- UI/UX refinement
- Testing
- Bug fixing
- Documentation
- Final presentation

---

## Project Timeline

The project is planned over **12 weeks**.

| Week | Main Activity |
|---|---|
| 1 | Requirements & Literature Review |
| 2 | System Design & UML |
| 3 | Proposal & UI Mockups |
| 4 | Landing & Authentication |
| 5 | Doctor Search |
| 6 | Appointment Booking |
| 7 | Queue Tracking |
| 8 | Patient & Doctor Dashboards |
| 9 | Admin Dashboard |
| 10 | UI/UX Refinement & Testing |
| 11 | Documentation & Bug Fixes |
| 12 | Final Presentation |

---

## Milestones

| Milestone | Output | Week |
|---|---|---|
| M1 | Requirements & Design Complete | 3 |
| M2 | Core UI Prototype | 6 |
| M3 | Booking & Queue Functional | 9 |
| M4 | Complete Prototype | 9 |
| M5 | Final Submission | 12 |

---

## Project Deliverables

The project deliverables include:

1. Project Proposal
2. Working Front-End Prototype
3. UML Documentation
4. DFD Documentation
5. Source Code
6. README Documentation
7. Final Presentation Slides
8. Live Demonstration

---

## Live Demo

**GitHub Pages:**  
https://iammoubee.github.io/software-engineering-and-project-management-project/

---


## Academic Information

**Project Title:** Medique — Smart Clinic Appointment & Queue Management System

**Course:** Capstone Project

**Department:** Department of ICT

**Session:** 2023–24

**Student:** Sadia Kabir Mou

**Student ID:** IT24016

---

## Conclusion

Medique provides a digital solution to common clinic problems such as unpredictable waiting times, manual token management, appointment scheduling difficulties, and lack of queue visibility.

The current prototype demonstrates the complete patient journey:

```text
Select Doctor
      ↓
Select Date & Time
      ↓
Book Appointment
      ↓
Receive Token
      ↓
Join Queue
      ↓
Track Queue
```

The project provides a foundation for developing a complete real-world clinic management system with backend services, database integration, real-time queue management, notifications, payments, and other advanced healthcare features.

---

## License

This project was developed as an academic capstone project for the **Department of ICT, Session 2023–24**.

© 2026 Medique — Smart Clinic Appointment & Queue Management System
