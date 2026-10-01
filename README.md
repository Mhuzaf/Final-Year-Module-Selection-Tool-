# Final Year Module Selection Tool

A JavaFX desktop application developed to help students manage their final-year module selections. The application allows students to create a profile, select their required modules, choose optional modules, reserve an optional module, and review their final selection through an overview screen.

## Overview

The Final Year Module Selection Tool provides a simple graphical interface for managing university module selections.

The application guides the user through several stages:

1. Create a student profile
2. Select a course
3. Select required and optional modules
4. Validate the total module credits
5. Reserve an optional module
6. Review the final selection
7. Save and load student data

The project was developed using Java and JavaFX with an object-oriented structure and an MVC-style separation between the model, views, and controller.

## Features

### Student Profile Management
- Create a student profile
- Enter student P number
- Enter first name and surname
- Enter email address
- Select a course
- Select a date
- Load existing student profile information

### Module Selection
- Display modules according to their block
- Separate Block 1, Block 2, and Block 3/4 modules
- Identify mandatory and optional modules
- Add optional modules to the selection
- Remove optional modules
- Reset module selections
- Track the student's current credit total
- Validate the required 120-credit selection

### Module Reservation
- Display available optional Block 3/4 modules
- Reserve an optional module
- Remove a reserved module
- Limit reservations to one optional module
- Confirm the reservation

### Selection Overview
- Display student profile information
- Display selected modules
- Display reserved modules
- Provide a final overview of the student's choices

### Data Persistence
- Save student data to a file
- Load previously saved student data
- Uses Java object serialization for persistence

## Technologies Used

- **Java**
- **JavaFX**
- **Object-Oriented Programming (OOP)**
- **MVC Architecture**
- **Java Collections**
- **Java Serialization**
- **Event-Driven Programming**
- **File I/O**

## Project Structure

The project is organised into model, view, and controller components.

```text
src/
├── controller/
│   └── ModuleChooserController.java
│
├── model/
│   ├── Block.java
│   ├── Course.java
│   ├── Module.java
│   ├── Name.java
│   └── StudentProfile.java
│
├── view/
│   ├── CreateStudentProfilePane.java
│   ├── ModuleChooserMenuBar.java
│   ├── ModuleChooserRootPane.java
│   ├── OverviewPane.java
│   ├── ReserveModulesPane.java
│   └── SelectModulesPane.java
│
└── application/
    └── ApplicationLoader.java
