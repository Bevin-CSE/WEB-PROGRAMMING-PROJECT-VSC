# VSC — Vehicle Service Center Management System

A frontend-only Web Programming mini project built with HTML, CSS and vanilla JavaScript. The project uses browser `localStorage` for demo records and `sessionStorage` for the current demo session. It does not use PHP, MySQL, or a server.

## Run locally
1. Extract the ZIP.
2. Open the `VSC_Vehicle_Service_Center` folder in VS Code.
3. Open `index.html` with Live Server, or open it directly in a browser.
4. Use one of the demo logins below.

## Demo login
All passwords are `12345`.

| Role | Email | Password |
|---|---|---|
| Customer | `user@gmail.com` | `12345` |
| Admin | `admin@gmail.com` | `12345` |
| Technician | `technision@gmail.com` | `12345` |

The dashboard shows the name of the currently logged-in demo user. You can also create customer and technician demo accounts from Signup.

## Main flow
1. Customer signs in and adds a vehicle if needed.
2. Customer books an appointment and enters the vehicle, service package, date, time slot, odometer and problem description.
3. The appointment appears in the Admin dashboard under Appointments & Approvals.
4. Admin reviews customer and vehicle details, chooses a technician, sees the technician's specialization/experience/availability, sets the expected delivery date and estimated cost, and approves.
5. Approval creates a Job Card linked to the appointment, customer and technician. It appears in the customer's Job Cards page and the technician's assigned jobs.
6. Technician updates status, diagnosis, work/tasks, cost and expected delivery. Those changes are visible in the customer dashboard.
7. Completing a job creates a demo invoice record. Customer can mark a demo payment as paid.
8. Admin can see customers, vehicles, technicians, job cards, billing and basic reports. Technicians can request demo spare parts.

## Source document alignment
The UI and basic workflows are based on the supplied *Vehicle Service Center Management System* document: Customer Master, Vehicle Master, Service Package Master, Appointment, Technician Master, Job Card, Job Task, Spare Part Master, Supplier Master, Purchase Order, Stock Transaction, Parts Request, Invoice, Payment, Customer Feedback and Service Reminder. The front-end mini project prioritizes the requested role-based appointment → approval → job-card flow and provides demo versions of parts requests, invoices/payments, feedback and reports.

## Important limitations
This is a college demonstration, not production software. Browser storage is local to the browser/device and is not shared across users or devices. Demo passwords are stored in browser storage and are not secure. Role checks in JavaScript are not real security. Email/SMS, payment gateway, Zoho Books, scheduled workflows, inventory automation and Blueprint enforcement from the original Zoho Creator project are not connected to external services in this version.
