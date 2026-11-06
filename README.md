# Teaching Assignment Management System

A collaborative Laravel web application for managing academic departments, teaching assignments, modules, faculty requests, and timetables.

## Overview

The system supports administrative and academic coordination workflows through role-based interfaces for administrators, department heads, coordinators, and professors.

## Features

- **Academic administration:** Manage departments, programs, students, professors, and user accounts.
- **Teaching coordination:** Manage modules, groups, teaching assignments, and visiting lecturers.
- **Faculty workflows:** Browse available modules, submit teaching preferences, and review assigned modules.
- **Timetables:** Create and edit schedules, view personal timetables, and export timetable documents.
- **Data exchange:** Import or export selected academic data using spreadsheet and PDF tooling.
- **Access control:** Authentication and role-based route authorization.

Features listed above are based on the application routes and dependencies; availability may depend on the configured user role and environment.

## Technology stack

- PHP 8.2+
- Laravel 12
- Blade templates, JavaScript, Bootstrap, Tailwind CSS
- Vite
- Laravel DOMPDF and Laravel Excel

## Local development

### Requirements

- PHP 8.2 or later
- Composer
- Node.js and npm
- A database supported by the application's Laravel configuration

### Setup

```bash
git clone https://github.com/mohssine0e/web-project.git
cd web-project

composer install
npm install

cp .env.example .env
php artisan key:generate
```

Configure your database connection and any required mail settings in `.env`, then run:

```bash
php artisan migrate
npm run dev
```

In a separate terminal, start the Laravel application:

```bash
php artisan serve
```

Depending on the workflow, you may also need to run `php artisan queue:work`. If the project relies on seed data or preconfigured roles, provision those before logging in.

## Collaboration

Developed collaboratively by [mohssine0e](https://github.com/mohssine0e) and [fahdcf](https://github.com/fahdcf).

## Project status

Academic project. This README documents the existing codebase; it is not a claim of production deployment or production readiness.
