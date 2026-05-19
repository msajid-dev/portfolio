# GratisGenieten — Voucher Marketplace & Affiliate Platform

**Client:** GratisGenieten, Netherlands &nbsp;·&nbsp; **Year:** 2025–2026

## Overview
High-traffic voucher and deals marketplace integrated with three major affiliate networks, with an AI-powered personalized recommendation engine.

## Architecture
```
gratisgenieten/
├── api/       Laravel 12 REST API
├── admin/     Next.js 16 admin panel
└── frontend/  Next.js 16 consumer portal
```

## My Role
- Engineered automated data feed ingestion from 3 affiliate networks: Daisycon, TradeTracker, TradeDoubler
- Built personalized recommendation engine using OpenAI + Pinecone vector search
- Implemented Mollie multi-gateway payment processing
- Built voucher catalog, user accounts, and redemption tracking

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend | Laravel 12, MySQL, Redis |
| Frontend | Next.js 16, TypeScript, Tailwind CSS |
| AI | OpenAI API, Pinecone vector DB |
| Payments | Mollie |
| Affiliate | Daisycon API, TradeTracker API, TradeDoubler API |

## Key Challenges
- **Affiliate feed sync:** Automated background jobs ingest and normalize product/voucher data from 3 different API formats
- **Recommendations:** User behavior embedded into Pinecone vectors; OpenAI ranks contextually relevant vouchers per user
