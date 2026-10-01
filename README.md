# campus-maintenance-reporting-system
# 🏫 Campus Maintenance Reporting System

A web-based platform that allows students and faculty to report campus maintenance and infrastructure issues and helps authorized staff track, manage, and resolve those issues efficiently.

## 📌 Overview

Campus maintenance problems such as broken lights, damaged classroom equipment, water leakage, Wi-Fi issues, cleanliness problems, and other infrastructure-related concerns are often reported through verbal communication or informal channels.

This makes it difficult to track reported issues, identify responsible departments, and know whether a problem has been resolved.

The **Campus Maintenance Reporting System** provides a centralized platform where users can report problems and authorized staff can manage and track them from a single dashboard.

## 🎯 Problem Statement

Students and faculty frequently encounter maintenance and infrastructure issues across the campus. These problems may be reported through different informal channels, making it difficult to maintain a proper record and track their resolution.

Our system provides a centralized platform for reporting, managing, and monitoring campus issues, improving communication between campus users and maintenance staff.

## 💡 Proposed Solution

The system allows students and faculty to:

* Report campus maintenance issues
* Select an issue category
* Provide location details
* Add a description of the problem
* Upload an optional image
* View reported issues
* Track issue status

Authorized staff or administrators can:

* View reported issues
* Search and filter issues
* Assign/manage reported issues
* Update issue status
* Monitor pending and resolved issues
* Manage maintenance requests through an admin dashboard

## ✨ Key Features

### 👨‍🎓 User Features

* User registration and login
* Report a maintenance issue
* Select issue category
* Enter campus location
* Add issue description
* Upload optional images
* View submitted reports
* Track issue status

### 👨‍💼 Admin Features

* Secure admin login
* Admin dashboard
* View all reported issues
* Search and filter issues
* Manage reported issues
* Update issue status
* Monitor pending and resolved issues

### 📊 Issue Status

Issues can move through the following stages:

`Reported → In Progress → Resolved`

## 🗂️ Issue Categories

The system can support categories such as:

* ⚡ Electrical
* 🚰 Plumbing
* 🪑 Classroom Equipment
* 🧹 Cleanliness
* 📶 Wi-Fi / Network
* 🏢 Infrastructure
* 🔧 Other Maintenance

## 🛠️ Technology Stack

### Frontend

* React.js
* JavaScript
* HTML
* CSS

### Backend

* Java
* Spring Boot
* Spring Security
* REST APIs

### Database

* MySQL

### Authentication

* JWT Authentication
* Spring Security

### Image Storage

* Cloudinary

### Deployment

* Vercel — Frontend
* Render — Backend

### Development & Collaboration

* Git
* GitHub
* Visual Studio Code

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │       Users         │
                    │ Students / Faculty  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   React Frontend    │
                    │  User/Admin Panels  │
                    └──────────┬──────────┘
                               │
                         REST API
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Spring Boot API   │
                    │  Business Logic &   │
                    │   Authentication    │
                    └──────────┬──────────┘
                               │
                    ┌──────────┴──────────┐
                    ▼                     ▼
             ┌──────────────┐      ┌──────────────┐
             │    MySQL     │      │  Cloudinary  │
             │   Database   │      │    Images    │
             └──────────────┘      └──────────────┘
```

## 📂 Project Structure

```text
campus-maintenance-reporting-system/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── main/
│   │   └── test/
│   └── pom.xml
│
├── docs/
│   ├── problem-statement.md
│   ├── requirements.md
│   └── architecture.md
│
├── README.md
└── .gitignore
```

## 👥 Team Members

| Name                | Role                     | Responsibilities                                                  |
| ------------------- | ------------------------ | ----------------------------------------------------------------- |
| **Aadrsh Patil**    | Team Lead & Tech Lead    | Backend, architecture, database integration, GitHub, coordination |
| **Basvaraj Hebbal** | Frontend & UI            | React frontend, UI design, dashboards, frontend integration       |
| **Arun Kumar M**    | Research & Documentation | Research, documentation, testing, presentation                    |

## 🚀 Development Plan

### Phase 1 — Planning

* Define requirements
* Finalize features
* Design system architecture
* Design database structure

### Phase 2 — Backend

* Create Spring Boot project
* Configure MySQL
* Create database entities
* Develop REST APIs
* Implement authentication
* Implement issue management

### Phase 3 — Frontend

* Create React application
* Build login/register pages
* Build issue reporting form
* Build user dashboard
* Build admin dashboard
* Integrate REST APIs

### Phase 4 — Testing

* Test user authentication
* Test issue submission
* Test image upload
* Test status updates
* Test search and filtering
* Fix bugs

### Phase 5 — Deployment

* Deploy frontend
* Deploy backend
* Configure database
* Configure environment variables
* Perform final testing

## 🔐 Security

The application will use:

* JWT-based authentication
* Spring Security
* Role-based access control
* Protected admin routes
* Secure API endpoints
* Environment variables for sensitive configuration

> Sensitive information such as database passwords, API keys, JWT secrets, and Cloudinary credentials will **not** be committed to GitHub.

## 📈 Future Enhancements

Possible future improvements include:

* Email notifications
* Push notifications
* Automatic department assignment
* Priority-based issue handling
* Duplicate issue detection
* Issue analytics and reports
* Maintenance staff mobile application
* QR codes for reporting issues at specific locations
* AI-assisted issue categorization
* SLA and resolution-time tracking

## 🎯 Expected Impact

The system aims to:

* Make campus issue reporting easier
* Reduce dependence on informal reporting channels
* Improve communication between users and maintenance staff
* Provide transparency through issue tracking
* Maintain a centralized record of maintenance requests
* Help administrators monitor unresolved issues

## 🤝 Contribution

This project is developed as a team project for a hackathon.

Team members should use Git branches for development and create pull requests before merging major changes into the main branch.

Example:

```bash
git checkout -b feature/issue-reporting
```

After completing the feature:

```bash
git add .
git commit -m "Add issue reporting feature"
git push origin feature/issue-reporting
```

Then create a Pull Request on GitHub.

## 📜 License

This project is currently developed for educational and hackathon purposes.

## ⭐ Project Status

🚧 **Currently in development**

More features and documentation will be added as the project progresses.

---

### 💻 Built with Java, Spring Boot, React, MySQL and teamwork.
