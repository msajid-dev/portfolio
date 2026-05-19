# United Medical Urgent Care — Clinic Management System

**Client:** United Medical Urgent Care, USA &nbsp;·&nbsp; **Year:** 2025

## Overview
Full-stack clinic management system for a US urgent care provider. Covers patient intake, appointment booking, doctor scheduling, and admin reporting.

## Architecture
```
united-medical-urgent-care/
├── api/     Laravel REST API
├── admin/   React admin panel (clinic staff)
└── web/     React patient web app
```

## My Role
- Architected and built the full system solo
- Designed the database schema for patient records, appointments, and billing
- Built REST API with Laravel Sanctum authentication
- Delivered React admin panel and patient-facing web app

## Tech Stack
Laravel 10 · React 18 · MySQL · REST API · Laravel Sanctum · Tailwind CSS

## Key Decisions
- Chose Laravel Sanctum over Passport for simpler SPA authentication
- Separated admin and patient apps into independent React projects for deployment flexibility
