Overview: Developed a comprehensive database schema and accompanying UI for managing patient information, appointments, reminders, and medical services. Ensured data integrity and relational consistency through normalized schema design up to 3NF.
Features:
Patients: Captures patient details including first name, last name, email, and phone number, with constraints to ensure at least one contact method is provided. Implements a function to raise an error if neither contact method is provided.
Appointments: Records appointment specifics with a one-to-many relationship with patients and reminders. Tracks appointment status and includes forms for CRUD operations.
Reminders: Manages appointment reminders, supporting both email and SMS types. Each reminder includes the patient's name, appointment details, and confirmation options.
Medical Services: Lists available medical services with a many-to-many relationship with patients, indicating the services each patient requires.
Entity-Relationship Diagram and Schema: Designed to meet 1NF, 2NF, and 3NF to ensure no partial or transitive dependencies.
Example Data and UI Implementation: Created sample data for patients, appointments, reminders, and services. Developed forms for creating, reading, updating, and deleting records across all entities.
