# Medicare System — Complete Hospital & Clinic Management

**Client:** Private (NDA) &nbsp;·&nbsp; **Year:** 2024–2025

## Overview
End-to-end hospital management platform covering patient registration, doctor scheduling, appointments, billing, pharmacy, and lab management — with dedicated mobile apps for doctors and patients.

## Architecture
```
medicare-system/
├── api/          Laravel REST API (backend)
├── admin/        React 18 admin panel (hospital staff)
├── web/          React patient-facing web app
├── doctor-app/   Flutter mobile app (doctors)
└── patient-app/  Flutter mobile app (patients)
```

## My Role
- Designed the full system architecture from scratch
- Built the Laravel REST API with role-based access (admin, doctor, patient, pharmacist, lab)
- Implemented appointment scheduling with conflict detection
- Built real-time notifications via Firebase Cloud Messaging
- Integrated payment gateway for billing
- Delivered all 5 components (API + 2 web apps + 2 Flutter apps)

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend API | Laravel 10, MySQL, Redis |
| Admin Panel | React 18, TypeScript, Tailwind CSS |
| Patient Web | React 18, Tailwind CSS |
| Mobile Apps | Flutter, Dart, Firebase |
| Auth | Laravel Sanctum, JWT |
| Notifications | Firebase Cloud Messaging |

## Key Challenges
- **Multi-role system:** Single API serving 5 different user types with isolated permissions
- **Appointment conflicts:** Built a scheduling engine that prevents double-booking across doctors and rooms
- **Offline mobile support:** Flutter apps cache critical data for areas with poor connectivity
