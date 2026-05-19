# Schepenkring — Real-Time Bidding & Auction Platform

**Client:** Schepenkring, Netherlands &nbsp;·&nbsp; **Year:** 2025–2026

## Overview
High-performance real-time auction platform with a live bidding engine and an automated multimedia generation pipeline that converts audit logs into video updates.

## Architecture
```
schepenkring/
├── api/       Laravel 12 REST API
├── admin/     Next.js 16 admin panel
└── frontend/  Next.js 16 bidder portal
```

## My Role
- Designed the real-time bidding engine using Pusher WebSockets for sub-second bid updates
- Built auction lifecycle management (listing → active → closed → settlement)
- Engineered automated video generation pipeline: audit logs → FFmpeg → OpenAI Sora → Yext distribution
- Implemented Pinecone vector search for auction item discovery

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend | Laravel 12, MySQL, Redis |
| Frontend | Next.js 16, TypeScript |
| Real-Time | Pusher WebSockets |
| AI / Media | OpenAI, OpenAI Sora, Pinecone, FFmpeg, Yext |
| Queue | Laravel Queues (video pipeline jobs) |

## Key Challenges
- **Bid latency:** Pusher WebSocket broadcasting keeps all connected clients in sync within milliseconds
- **Video pipeline:** Background queue jobs process audit logs → generate video via Sora → distribute via Yext automatically
