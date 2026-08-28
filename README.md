# Employee Management System (HRMS)

A full-featured Human Resource Management System built with **ASP.NET Core MVC**, **C#**, **Entity Framework Core**, and **Microsoft SQL Server**. Designed to streamline core HR operations — from employee onboarding to payroll — with secure, role-based access for administrators, HR staff, and employees.

![.NET](https://img.shields.io/badge/.NET-8.0-512BD4?logo=dotnet)
![C#](https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?logo=microsoftsqlserver&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📌 Overview

HRMS is a centralized platform for managing an organization's workforce. It replaces manual, spreadsheet-driven HR processes with a secure web application that handles employee records, attendance, leave requests, payroll, and departmental structure — with a full audit trail for accountability.

## ✨ Features

- **Employee Management** — Create, update, and maintain detailed employee profiles
- **Attendance Tracking** — Record and monitor daily employee attendance
- **Leave Management** — Submit, approve, and track leave requests
- **Payroll Processing** — Manage salary structures and payroll generation
- **Departments & Designations** — Organize employees by department and job role
- **Authentication & Authorization** — Secure login with role-based access control (Admin / HR / Employee)
- **Audit Logging** — Track key actions across the system for accountability and compliance

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | ASP.NET Core MVC, C# |
| Data Access | Entity Framework Core |
| Database | Microsoft SQL Server |
| Frontend | HTML, CSS, Bootstrap |

## 🏗️ Architecture

The project follows the **MVC (Model-View-Controller)** pattern with a layered approach:

```
HRMS/
├── Controllers/     # Handle HTTP requests and business logic flow
├── Models/          # Domain entities and EF Core data models
├── Views/           # Razor views (UI)
├── Data/            # DbContext, migrations, seed data
├── Services/        # Business logic / reusable services
└── wwwroot/         # Static assets (CSS, JS, images)
```

## 🚀 Getting Started

### Prerequisites

- [.NET SDK 8.0+](https://dotnet.microsoft.com/download)
- [SQL Server](https://www.microsoft.com/sql-server) (or SQL Server Express / LocalDB)
- Visual Studio 2022 or VS Code

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/velpulasaitharun/Employee-Management-System.git
   cd Employee-Management-System
   ```

2. **Configure the database connection**

   Update the connection string in `appsettings.json`:
   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=YOUR_SERVER;Database=HRMSDb;Trusted_Connection=True;TrustServerCertificate=True;"
   }
   ```

3. **Apply migrations**
   ```bash
   dotnet ef database update
   ```

4. **Run the application**
   ```bash
   dotnet run
   ```

5. Open your browser at `https://localhost:5001` (or the port shown in your terminal).

## 📸 Screenshots

> _Add screenshots of the dashboard, employee list, and login page here to give visitors a quick visual tour._

## 🗺️ Roadmap

- [ ] Add unit and integration tests
- [ ] Add employee self-service portal enhancements
- [ ] Add email notifications for leave approvals
- [ ] Deploy a live demo

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](../../issues) or open a pull request.

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Sai Tharun Velpula**
- GitHub: [@sai-tharun-velpula](https://github.com/sai-tharun-velpula)
