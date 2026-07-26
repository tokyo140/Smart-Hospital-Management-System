# Smart Hospital Queue & Triage Management System

A web-based Healthcare Management System designed to reduce overcrowding in government hospitals by digitizing patient queues, enabling smart appointment booking, and prioritizing patients based on urgency — ensuring every patient gets timely and proper treatment.

## Problem Statement

Government hospitals often face heavy overcrowding due to walk-in patients, lack of proper triage, and no visibility into wait times. This leads to long queues, delayed treatment for urgent cases, and inefficient use of hospital resources. This project aims to solve this by introducing a digital queue and triage system.

## Objectives

- Reduce physical crowding by enabling online appointment booking
- Route patients to the correct department based on symptoms
- Prioritize patients using an urgency-scoring system, not just first-come-first-served
- Give patients real-time visibility into queue position and estimated wait time
- Give hospital staff a live dashboard to manage patient flow efficiently

## Features

### Patient Side
- Register/login
- Book appointments by selecting symptoms (auto-suggests relevant department)
- Get a digital token number with live queue position and estimated wait time
- View, cancel, or reschedule appointments

### Staff Side
- Login for doctors/receptionists
- View live department-wise queue, sorted by urgency and arrival time
- Update patient status (waiting / in-progress / done)

### Admin Side
- Manage departments and staff
- View overall hospital load and basic analytics (patients per day, average wait time, peak hours)

## Tech Stack

- **Backend:** Django, Django REST Framework
- **Frontend:** React.js
- **Database:** SQLite (development) / PostgreSQL (production)
- **Version Control:** Git & GitHub

## Database Design

The system is built around five core entities: Users, Departments, Staff, Appointments, and Queue Logs. See `docs/er_diagram.png` for the full entity-relationship diagram.

## Project Status

🚧 Work in progress — currently in initial backend setup phase.

## Setup Instructions

```bash
# Clone the repository
git clone https://github.com/tokyo140/smart-hospital-management.git
cd smart-hospital-management

# Create and activate virtual environment
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # Mac/Linux

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start development server
python manage.py runserver
```

## Author
tokyo140

