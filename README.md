
# Student-Teacher Booking Appointment System

This is a MERN stack project designed to facilitate the booking of appointments between students and teachers. The system includes functionalities for admins to manage teachers, for teachers to manage their appointments, and for students to book appointments with teachers.

## Table of Contents
- [Features](#features)
- [System Modules](#system-modules)
  - [Admin](#admin)
  - [Teacher](#teacher)
  - [Student](#student)
- [Tech-Stack-Used](#tech-stack-used)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Login Acess](#login)
- [Contributing](#contributing)

## Features
- Admin management for adding, updating, and deleting teachers and approving student registrations.
- Teacher functionalities for managing their appointment schedules, approving/cancelling appointments, sending email alerts to students, viewing messages, and viewing all appointments.
- Student functionalities for registering, booking appointments with teachers, sending email alerts to teachers, and sending messages.

## System Modules

### Admin
- Add Teacher (Name, Department, Subject, etc.)
- Update/Delete Teacher
- Approve Registration Student

### Teacher
- Login
- Schedule Appointment
- Approve/Cancel Appointment
- Send Email Alerts to Students
- View Messages
- View All Appointments

### Student
- Register
- Login
- Book Appointment
- Send Email Alert to Teacher
- Send Message

## Tech-Stack-Used

**Frontend**
```bash
vite (bundler-react)
tailwindcss (styling)
react-icons (icons)
react-router-dom (routing)
react-toastify (notify)
axios (API)
```
**Backend**
```bash
express (API)
jwt-token (token)
nodemail (MAIL)
bcrypt (encryption)
```

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/rudrax14/MERN_STACK-StudentTeacher-Booking-Appointment
    ```

2. **Install backend dependencies:**
    ```bash
    cd backend
    npm install
    ```

3. **Install frontend dependencies:**
    ```bash
    cd frontend
    npm install
    ```

4. **Set up environment variables for the backend:**

    Create a `.env` file in the `backend` directory with the following content:
    ```env
    DB_URL=''
    JWT_KEY = ''
    PORT = 5000

    # mail integration 

    MAIL_HOST = smtp.gmail.com
    MAIL_USER = 'your_mail'
    MAIL_PASS = 'your_pass'
    ```

5. **Run the backend server:**
    ```bash
    cd backend
    npm run dev
    ```

6. **Run the frontend server:**
    ```bash
    cd frontend
    npm run dev
    ```
7. **Set up environment variables for frontend:**

    Create a `.env.local` file in the `frontend` directory with the following content:
    ```env
    VITE_BACKEND_URL='http://localhost:5000'
    ``` 

The application should now be running on `http://localhost:5173/`.

## Usage

1. **Admin:**
    - Log in to the admin dashboard.
    - Add, update, or delete teachers.
    - Approve student registrations.

2. **Teacher:**
    - Log in to the teacher portal.
    - Schedule, approve, or cancel appointments.
    - Send email alerts to students.
    - View messages and all appointments.

3. **Student:**
    - Register and log in to the student portal.
    - Book appointments with teachers.
    - Send email alerts and messages to teachers.

## Screenshots

Landing Page 

![landingpage Dark](https://private-user-images.githubusercontent.com/165495553/460201164-71b8f8e1-1643-4a8b-947a-cf4255904cb0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTEwODcwMTQsIm5iZiI6MTc1MTA4NjcxNCwicGF0aCI6Ii8xNjU0OTU1NTMvNDYwMjAxMTY0LTcxYjhmOGUxLTE2NDMtNGE4Yi05NDdhLWNmNDI1NTkwNGNiMC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDYyOFQwNDU4MzRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hNzlhNGEzYjg4NDk5MGIxMzFlMGQ0MWNjNTc2NTZkODVjMWJiNGFkMDUyZmYwMmQ3NzlhZTg3ZmU0YTg3ZTAwJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.TSUWBk2FbE2QYkhcRzV4k1gbYnGAGRreekloS1GDv5c)

Student Dashboard

![student dashboard dark](https://private-user-images.githubusercontent.com/165495553/460203348-8775d2c2-f665-408b-a90e-eb0b9ccde79b.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTEwOTAyNzYsIm5iZiI6MTc1MTA4OTk3NiwicGF0aCI6Ii8xNjU0OTU1NTMvNDYwMjAzMzQ4LTg3NzVkMmMyLWY2NjUtNDA4Yi1hOTBlLWViMGI5Y2NkZTc5Yi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDYyOFQwNTUyNTZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05YTg5OGYzMDYzYTRmZjIwZTdkZDk3ODM3MjJjMjkxNzViNWRkODlkZjYxY2FmMThhZGU5ZDk5YjYzNGNmZDNkJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.PZlGybt-ywCkxefV7-OUeSnIDm3_ESi-eDzd61AIaOs)

Teacher Dashboard

![teacher d Dark](https://private-user-images.githubusercontent.com/165495553/460203742-3202c1a9-bae7-4062-88a2-221006bfbef5.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTEwOTAzODYsIm5iZiI6MTc1MTA5MDA4NiwicGF0aCI6Ii8xNjU0OTU1NTMvNDYwMjAzNzQyLTMyMDJjMWE5LWJhZTctNDA2Mi04OGEyLTIyMTAwNmJmYmVmNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDYyOFQwNTU0NDZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05MDliNWRhMTkzZmU5Y2ZlMDBiODNkNjFlODZiNTA1OWU5Y2U0MjZiZjNmMjc1NzQxYjFmZGRiZjgxMTNjY2NiJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.CP0U9gwgnKDE-AONDQWRGjmhOFqmBFjZcrx7b-acx0U)


Admin Dashboard

![admin ](https://private-user-images.githubusercontent.com/165495553/460203754-9227f6c9-4dba-4b47-a823-eb2ee67f7d5c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTEwOTA1ODcsIm5iZiI6MTc1MTA5MDI4NywicGF0aCI6Ii8xNjU0OTU1NTMvNDYwMjAzNzU0LTkyMjdmNmM5LTRkYmEtNGI0Ny1hODIzLWViMmVlNjdmN2Q1Yy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDYyOFQwNTU4MDdaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0xOTRlMzIzZDljNTRlZmZhOTRiOGYxYTVhMjNhZmVlNzBlZTdlOGYwNjE0N2Y0MDg0MDljZWEzODMzNTJlMmE4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.IMNUm1qNZS6LPojjYFhyPd1WZMNeWsFkygOekzvlY2w)

## Login

**Student**
 ```bash
email: student@gmail.com
Password: student123
 ```
**Teacher**
 ```bash
email: teacher@gmail.com
Password: teacher123
 ```
**Admin**
 ```bash
email: admin@gmail.com
Password: admin
 ```
**Note: Don't Spam**

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create your feature branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a pull request.

## Thank You 

**Keep Coding**
