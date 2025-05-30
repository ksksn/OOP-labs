# OOP-labs

# Student Record Management System

## Description
This project is a console-based **Student Record Management System** developed using **Layered Architecture** principles. It allows users to manage student records by adding, editing, and viewing student information. Additionally, after adding a new student, the system fetches and displays a motivational quote using the **quotable.io API**.

## Author
**YOUR NAME**  
**Group: YOUR GROUP NUMBER**

## Features
- Add, edit, and view student records.
- Input validation for student data (name and grade).
- In-memory storage of records in a JSON file.
- Fetch and display a motivational quote after adding a student.

## Architecture
The system is designed using a **Layered Architecture** with the following layers:
- **Presentation Layer**: Handles user input and output via the console.
- **Application Layer**: Manages business logic and coordination between layers.
- **Domain Layer**: Represents core data and validation (Student entity and Quote validation).
- **Data Access Layer**: Manages data persistence using an in-memory repository.

## Data Transfer Objects (DTOs)
- **StudentDTO**: Used to transfer validated student data from the UI to the service.
- **QuoteDTO**: Used to transfer the motivational quote fetched from the API.

## Design Patterns
- **Behavioral Pattern**: Command pattern for handling student operations (add, edit, view).
- **Structural Pattern**: Adapter pattern for calling the external quote API.
- **Creational Pattern**: Factory method for creating `Student` and `QuoteDTO` objects.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
   cd YOUR_REPOSITORY
