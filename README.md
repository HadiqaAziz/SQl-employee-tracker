
# SQL Employee Tracker

Welcome to the SQL Employee Tracker repository! This project provides a command-line application that helps you manage departments, roles, and employees within your company. Follow the steps below to get started.

## Table of Contents
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Installation](#installation)
- [Usage](#usage)
- [Video Demonstration](#video-demonstration)

## User Story

As a business owner, you need a tool to effectively view and manage the departments, roles, and employees in your company. This application allows you to organize and plan your business operations efficiently.

## Acceptance Criteria

The application fulfills the following criteria:

- **GIVEN** a command-line application that accepts user input
  - **WHEN** you start the application
    - **THEN** you are presented with the following options:
      - View all departments
      - View all roles
      - View all employees
      - Add a department
      - Add a role
      - Add an employee
      - Update an employee role

- **WHEN** you choose to view all departments
  - **THEN** you are presented with a formatted table showing department names and department IDs.

- **WHEN** you choose to view all roles
  - **THEN** you are presented with the job title, role ID, the department that role belongs to, and the salary for that role.

- **WHEN** you choose to view all employees
  - **THEN** you are presented with a formatted table showing employee data, including employee IDs, first names, last names, job titles, departments, salaries, and managers that the employees report to.

- **WHEN** you choose to add a department
  - **THEN** you are prompted to enter the name of the department, and that department is added to the database.

- **WHEN** you choose to add a role
  - **THEN** you are prompted to enter the name, salary, and department for the role, and that role is added to the database.

- **WHEN** you choose to add an employee
  - **THEN** you are prompted to enter the employee’s first name, last name, role, and manager, and that employee is added to the database.

- **WHEN** you choose to update an employee role
  - **THEN** you are prompted to select an employee to update, choose their new role, and this information is updated in the database.

## Installation

To install and run the SQL Employee Tracker application, follow these steps:

1. Clone this repository to your local machine.
    ```bash
    git clone https://github.com/HadiqaAziz/SQL-employee-tracker.git
    ```
2. Navigate to the project directory.
    ```bash
    cd SQL-employee-tracker
    ```
3. Install the necessary dependencies.
    ```bash
    npm install
    ```
4. Set up the database:
    - Log in to your MySQL server.
    - Run the provided SQL script to create the database and tables.
    ```sql
    SOURCE db/schema.sql;
    ```

5. Seed the database with initial data (optional).
    ```sql
    SOURCE db/seeds.sql;
    ```

6. Start the application.
    ```bash
    node index.js
    ```

## Usage

After starting the application, you will be presented with a menu of options. Simply use the arrow keys to navigate through the options and press `Enter` to select one. Follow the prompts to view, add, or update information in the database.

Here are some of the main operations you can perform:

- **View all departments**: Displays a list of all departments in your company.
- **View all roles**: Shows all roles along with the corresponding department and salary.
- **View all employees**: Lists all employees with their job titles, departments, and managers.
- **Add a department**: Allows you to add a new department to the database.
- **Add a role**: Enables you to create a new role by specifying its name, salary, and department.
- **Add an employee**: Lets you add a new employee by entering their personal and job details.
- **Update an employee role**: Helps you update an employee’s role within the company.

## Video Demonstration

For a step-by-step walkthrough of the application, check out the [video demonstration](https://drive.google.com/file/d/1g3g2Vrar_UcnNAd5VdEbXKkIN4dpL3LC/view).

For any issues or questions, feel free to open an issue in the repository.
