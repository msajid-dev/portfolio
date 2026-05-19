# Medicare System — Complete Hospital & Clinic Management

**Client:** Private (NDA) &nbsp;·&nbsp; **Year:** 2024–2025

## Overview
End-to-end hospital management platform covering patient registration, doctor scheduling, appointments, billing, pharmacy, and lab management.

## Architecture
```
medicare-system/
├── api/    Laravel REST API (backend)
├── admin/  React 18 admin panel (hospital staff)
└── web/    React patient-facing web app
```

## My Role
- Designed the full system architecture
- Built the Laravel REST API with role-based access (admin, doctor, patient, pharmacist, lab)
- Implemented appointment scheduling with conflict detection
- Integrated payment gateway for billing
- Built React admin panel and patient web app

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend API | Laravel 10, MySQL, Redis |
| Admin Panel | React 18, TypeScript, Tailwind CSS |
| Patient Web | React 18, Tailwind CSS |
| Auth | Laravel Sanctum |
| Notifications | Firebase Cloud Messaging |

## Key Challenges
- **Multi-role system:** Single API serving 5 different user types with isolated permissions
- **Appointment conflicts:** Scheduling engine that prevents double-booking across doctors and rooms
