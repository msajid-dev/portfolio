# MAANUM — Standalone eCommerce Platform

**Client:** Private &nbsp;·&nbsp; **Year:** 2025

## Overview
Solo-built eCommerce platform with advanced cart synchronization, multi-gateway payments, real-time support, and AI-powered customer service.

## Architecture
```
manal-store/
├── api/    Laravel 12 REST API
├── admin/  React 19 admin dashboard
└── store/  React 19 customer storefront
```

## My Role
- Architected and built the entire platform solo
- Implemented fully cross-tab synchronized shopping cart with guest session merging on login
- Integrated 5 payment gateways: Stripe, digital mobile wallets, cash on delivery, and local gateways
- Built real-time admin support chat using WebSockets
- Implemented AI-powered automated customer service bot
- Built image processing pipeline for product media

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend | Laravel 12, MySQL, Redis |
| Frontend | React 19, Tailwind CSS |
| Real-Time | WebSockets, Laravel Echo |
| AI | OpenAI API |
| Payments | Stripe + 4 additional gateways |

## Key Challenges
- **Cross-tab cart sync:** BroadcastChannel API keeps cart state consistent across all open browser tabs in real time
- **Guest merge:** On login, anonymous cart seamlessly merges with authenticated user cart without data loss
