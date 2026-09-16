# FY--Assignment--Team-10
ER Diagram – Clinic Appointment Booking System
About
This folder contains the Entity Relationship (ER) Diagram for the BCA project "Clinic – Appointment Booking System", drawn using Crow's Foot notation on a clean academic white/light-blue background.
File: er_diagram.svg (SVG is a scalable vector format — it stays sharp at any zoom level or print size, and can be opened directly in a browser, or imported into Word/PowerPoint.)
Entities and Attributes
1. PATIENT
Attribute
Key
Patient_ID
Primary Key (PK)
Patient_Name
—
Age
—
Gender
—
Contact_Number
—
2. DOCTOR
Attribute
Key
Doctor_ID
Primary Key (PK)
Doctor_Name
—
Specialization
—
Available_Time
—
3. APPOINTMENT
Attribute
Key
Appointment_ID
Primary Key (PK)
Patient_ID
Foreign Key (FK) → references PATIENT
Doctor_ID
Foreign Key (FK) → references DOCTOR
Appointment_Date
—
Appointment_Time
—
Booking_Status
—
Relationships & Cardinality
PATIENT (1) ────< (M) APPOINTMENT (M) >──── (1) DOCTOR
One PATIENT books many APPOINTMENTs (1:M) — each Appointment belongs to exactly one Patient.
One DOCTOR is assigned to many APPOINTMENTs (1:M) — each Appointment is assigned to exactly one Doctor.
APPOINTMENT is the associative/junction entity connecting PATIENT and DOCTOR, holding both foreign keys.
Notation Key
Bold + underlined attribute = Primary Key (PK)
Italic attribute = Foreign Key (FK)
Two parallel ticks (⊣⊣) on a connector = "exactly one" (1)
Crow's foot (fan of 3 lines) on a connector = "many" (M)
How to Use
Open er_diagram.svg in any web browser to view it full-size, or insert it directly into a Word document / PowerPoint slide (Insert → Pictures) for your assignment or presentation.
Since it's vector-based, it can be resized freely without losing quality when printed.
Design Notes
Rectangular boxes represent entities; header bars are colour-coded in academic blue for a clean, professional look.
The diagram deliberately includes only the three entities and attributes specified — no extra entities or attributes were added.
A legend at the bottom explains PK/FK styling and Crow's Foot cardinality symbols for anyone reviewing the diagram.
Clinic – Appointment Booking System
Algorithm
Modules: Patient Details, Doctor Details, Appointment, Appointment Date and Time
Step-by-Step Algorithm
START
Enter Patient Details
Patient ID
Patient Name
Age
Gender
Contact Number
Enter/Select Doctor Details
Doctor ID
Doctor Name
Specialization
Available Time
Select Doctor from the list of available doctors (based on Specialization)
Select Appointment Date and Time
Check Doctor Availability for the selected Date and Time
Decision: Is the Doctor Available?
If NO: 7.1 Display message "Doctor Not Available" 7.2 Prompt user to select another Date/Time 7.3 Go to Step 5
If YES: 7.4 Proceed to Step 8
Create Appointment
Generate Appointment ID
Store Patient ID
Store Doctor ID
Store Appointment Date
Store Appointment Time
Set Booking Status = "Confirmed"
Display Appointment Details
Appointment ID
Patient Name
Doctor Name
Specialization
Appointment Date
Appointment Time
Booking Status
END
Summary Flow
START → Enter Patient Details → Select Doctor → Select Date/Time → Check Availability → (NO → Retry) → (YES → Create Appointment → Confirm Status → Display Details) → END
Clinic – Appointment Booking System | Flowchart
Project Overview
This project is a BCA college assignment for a Clinic – Appointment Booking System.
The flowchart represents the complete appointment-booking process, from entering patient and doctor information to confirming and displaying the appointment.
Flowchart Process
START
Enter Patient Details
Patient ID
Patient Name
Age
Gender
Contact Number
Enter Doctor Details
Doctor ID
Doctor Name
Specialization
Available Time
Select Doctor
Select Appointment Date & Time
Check Doctor Availability
Decision: Is the Doctor Available?
NO: Display “Doctor Not Available” → Select another Date/Time → Check Availability again
YES: Continue to create the appointment
Create Appointment
Set Booking Status = Confirmed
Display Appointment Details
Patient
Doctor
Date
Time
Booking Status
END
Flowchart Symbols
Symbol
Meaning
Oval
Start / End
Rectangle
Process
Diamond
Decision
Parallelogram
Input / Output
Arrow
Flow Direction
Design Guidelines
Use a clean, professional academic design suitable for a BCA student.
Use a white/light-blue background with a subtle gradient.
Use readable fonts and consistent spacing.
Clearly label decision branches as YES and NO.
Keep arrows clear and avoid crossing lines.
Add small professional icons for:
Patient
Doctor
Calendar
Clock
Appointment
Keep the design modern, neat, and suitable for:
College submission
Viva
Classroom presentation
Printing
Suggested Color Scheme
🔵 Blue: Patient Details
🟢 Green: Doctor Details
🟣 Purple: Appointment Date & Time
🟠 Orange: Availability Decision
🔷 Teal: Appointment Confirmation
🔴 Red: Not Available / Error
⚫ Dark Blue: START and END
Objective
The objective of this flowchart is to clearly visualize how a clinic appointment is booked, how doctor availability is checked, and how a confirmed appointment is generated and displayed.
Expected Outcome
The system should provide a simple and understandable appointment-booking workflow in which:
Patient information is entered.
Doctor information is entered and a doctor is selected.
Appointment date and time are selected.
Doctor availability is checked.
An unavailable slot allows the user to select another date/time.
An available slot creates and confirms the appointment.
Final appointment details are displayed.
Assignment Title
Clinic – Appointment Booking System
Diagram: Flowchart
Academic Level: BCA
Purpose: College Assignment / Project Documentation
