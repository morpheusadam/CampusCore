<div align="center">

# 🎓 Iranian University — Laravel University Management System

### A comprehensive **university / college management system** built with **Laravel 10** — manage students, professors, colleges, courses, classes, terms, schedules, attendance, and roles, with Jalali (Persian) calendar support.

<p>
  <img src="https://img.shields.io/github/license/morpheusadam/iranian-univercity?style=for-the-badge&color=4c1" alt="License" />
  <img src="https://img.shields.io/github/stars/morpheusadam/iranian-univercity?style=for-the-badge&color=ffca28" alt="Stars" />
  <img src="https://img.shields.io/github/forks/morpheusadam/iranian-univercity?style=for-the-badge&color=42a5f5" alt="Forks" />
  <img src="https://img.shields.io/github/last-commit/morpheusadam/iranian-univercity?style=for-the-badge&color=8e44ad" alt="Last commit" />
  <img src="https://img.shields.io/github/repo-size/morpheusadam/iranian-univercity?style=for-the-badge&color=e67e22" alt="Repo size" />
</p>

<p>
  <img src="https://img.shields.io/badge/Laravel-10-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PHP-8.1%2B-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Bootstrap-UI-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap" />
  <img src="https://img.shields.io/badge/Vite-Build-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Spatie-Permissions-4B5563?style=for-the-badge&logo=php&logoColor=white" alt="Spatie Permission" />
</p>

</div>

---

## 📖 Overview

**Iranian University** is a comprehensive **university management system** built with the **Laravel 10** framework. It gives academic institutions a single platform to manage their core entities — students, professors, colleges (faculties), educational groups, courses/lessons, classrooms, locations, academic terms, time periods, schedules, and attendance.

The system ships with **role-based access control** (powered by Spatie Laravel Permission) covering distinct roles such as **Admin, Faculty Head, Educational Supervisor, and Professor**, each guarded by dedicated middleware. It supports the **Jalali (Persian) calendar** via `morilog/jalali`, and can generate documents through **PHPWord** and **PDF** export, making it well-suited to Iranian and other RTL-oriented academic environments.

It's a solid foundation for **developers and institutions** that need a customizable Laravel-based academic information / student management system.

> 🔎 **Keywords:** university management system, student management, laravel education, college management, course scheduling, attendance system, role-based access, spatie permission, jalali calendar, persian university software.

---

## ✨ Features

- 👨‍🎓 **Student registration & management**
- 👩‍🏫 **Professor & staff management**
- 🏛️ **College (faculty) & educational group management**
- 📚 **Course / lesson creation & management**
- 🚪 **Classroom & location management**
- 🗓️ **Academic terms & time periods**
- ⏰ **Scheduling & timetables**
- ✅ **Presence & absence (attendance) tracking**
- 🔐 **Role-based access control** — Admin, Faculty Head, Educational Supervisor, Professor
- 📝 **Entry/enrollment management**
- 📄 **Document & report generation** (PHPWord / PDF)
- 🌍 **Jalali (Persian) calendar support**

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=laravel,php,mysql,bootstrap,vite,sass,js" alt="Tech stack" />
</p>

| Layer | Technologies |
| --- | --- |
| Backend | Laravel 10, PHP 8.1+, Laravel Sanctum, Tinker |
| Authorization | Spatie Laravel Permission (roles & permissions) |
| Frontend | Blade, Bootstrap, Bootstrap Icons, Select2, jQuery, Sass, Vite |
| Documents | morilog/jalali (Persian dates), PHPWord, misterspelik/laravel-pdf |
| Forms | LaravelCollective HTML, Laravel UI |

---

## 🚀 Getting Started

### Prerequisites

- **PHP 8.1+** with Composer
- **MySQL** (or PostgreSQL)
- **Node.js & npm** (for frontend assets)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/morpheusadam/iranian-univercity.git
cd iranian-univercity

# 2. Install dependencies
composer install
npm install
npm run dev

# 3. Configure environment
cp .env.example .env
php artisan key:generate

# 4. Set your database credentials in .env, then migrate & seed
php artisan migrate --seed

# 5. Serve the application
php artisan serve
```

### Usage

1. Open `http://localhost:8000` in your browser.
2. Log in (or register), then use the dashboard to manage students, professors, colleges, courses, schedules, and attendance.
3. Access is governed by roles — Admin, Faculty Head, Educational Supervisor, and Professor each see the tools relevant to them.

---

## 🗂️ Project Structure

```text
iranian-univercity/
├── app/
│   ├── Http/Controllers/   # ClassRoom, Collage, EducationalGroup,
│   │                       # Professor, Lesson, Schedule, Term,
│   │                       # PresenceAndAbsence, Entry, User...
│   ├── Http/Middleware/    # Admin, FacultyHead, EducationalSupervisor,
│   │                       # Professor, Role, TermExists...
│   ├── Models/             # Collage, Professor, Term, Classroom,
│   │                       # Lesson, Location, presenceAndAbsence...
│   └── Providers/
├── config/                 # configuration files
├── resources/              # Blade views & frontend assets
└── routes/                 # route definitions
```

---

## 🤝 Contributing

Contributions are welcome! Open an [issue](https://github.com/morpheusadam/iranian-univercity/issues) or submit a pull request with new features, fixes, or improvements.

## 📜 License

Built on the open-source **Laravel** framework (MIT). Add a `LICENSE` file to clarify distribution terms.

---

<div align="center">

### 👤 Author — Morpheus Adam

Web developer & cheerful hacker · PHP · Laravel · Go

<p>
  <a href="https://github.com/morpheusadam"><img src="https://img.shields.io/badge/GitHub-morpheusadam-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://sam.zeonic.me"><img src="https://img.shields.io/badge/Website-sam.zeonic.me-4c1?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="mailto:morpheusadam95@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

⭐ **If this project helped you, please give it a star!** ⭐

</div>
