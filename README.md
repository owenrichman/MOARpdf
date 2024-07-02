## Overview
Developed a comprehensive database schema and accompanying UI for managing patient information, appointments, reminders, and medical services. Ensured data integrity and relational consistency through normalized schema design up to 3NF.

## Features

### Patients
- **Details Captured:** First name, last name, email, and phone number.
- **Constraints:**
  - At least one contact method (email or phone) must be provided.
  - Function to raise an error if neither contact method is provided.

### Appointments
- **Details Recorded:** Appointment specifics, including status.
- **Relationships:**
  - One-to-many with patients (one patient can have multiple appointments).
  - One-to-many with reminders (one appointment can have multiple reminders).
- **CRUD Operations:** Forms for creating, reading, updating, and deleting appointments.

### Reminders
- **Details Managed:** Reminders for each patient.
- **Types Supported:** Email and SMS.
- **Content:** Includes patient's name, appointment date/time, service description, and options to confirm or cancel the appointment.
- **Relationship:** Many-to-one with appointments (multiple reminders can relate to one appointment).

### Medical Services
- **Details Listed:** Various medical services available for booking.
- **Relationships:**
  - Many-to-many with patients (each service can have multiple patients and vice versa).

## Entity-Relationship Diagram and Schema
Designed to meet the following normal forms:
- **1NF:** Each table has a primary key, and all attributes are dependent on that key.
- **2NF:** Each table meets 1NF and has no partial dependencies.
- **3NF:** Each table meets 2NF and contains no transitive dependencies.

## Example Data and UI Implementation
- **Sample Data:** Created for patients, appointments, reminders, and services.
- **UI Features:** Developed forms for creating, reading, updating, and deleting records across all entities.
