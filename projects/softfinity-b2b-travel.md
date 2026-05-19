# Softfinity B2B Travel Portal

**Client:** Softfinity Solutions &nbsp;·&nbsp; **Year:** 2024–2025

## Overview
B2B travel portal for travel agencies to search, book, and manage flights and hotels. Includes a Next.js admin dashboard and a React-based agent-facing frontend.

## Architecture
```
softfinity-b2b-travel/
├── api/       Laravel REST APIs (flights, hotels, bookings, agents)
├── admin/     Next.js admin dashboard
└── frontend/  React agent portal
```

## My Role
- Designed multi-API architecture integrating third-party flight and hotel providers
- Built agent management system with credit limits and commission tracking
- Implemented booking workflow with hold, confirm, and cancel states
- Built voucher generation and PDF export

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend | Laravel, MySQL, Redis (queue jobs) |
| Admin | Next.js, TypeScript |
| Agent Portal | React 18, Tailwind CSS |
| Background Jobs | Laravel Queues (booking confirmations, emails) |
| PDF | Laravel DomPDF |

## Key Challenges
- **Third-party API reliability:** Implemented retry logic and fallback caching for flight search results
- **Credit system:** Real-time credit deduction with rollback on booking failure
