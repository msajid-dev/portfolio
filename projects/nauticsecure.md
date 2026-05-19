# NauticSecure — Digital Asset Marketplace & Transaction Management

**Client:** NauticSecure, Netherlands &nbsp;·&nbsp; **Year:** 2025–2026

## Overview
Secure high-value digital asset marketplace with automated KYC onboarding, a strict transaction state machine (bid → deposit → escrow → contract), and an AI-powered omni-channel communication inbox.

## Architecture
```
nauticsecure/
├── api/       Laravel 12 REST API
├── admin/     Next.js 16 admin panel
└── frontend/  Next.js 16 buyer/seller portal
```

## My Role
- Designed and built the full system architecture
- Built the transaction state machine: bid → deposit handling → escrow → contract execution
- Integrated Signhost for digital contract signing and seller KYC onboarding
- Built omni-channel messaging inbox combining WhatsApp, SMS, email, and voice calls
- Implemented AI RAG copilot using OpenAI + Pinecone for contextual support
- Real-time features via WebSockets

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Backend | Laravel 12, MySQL, Redis |
| Frontend | Next.js 16, TypeScript, Tailwind CSS |
| Real-Time | WebSockets, Laravel Echo |
| AI | OpenAI API, Pinecone vector DB (RAG) |
| Payments | Mollie |
| KYC / Contracts | Signhost |
| Messaging | WhatsApp API, SMS, Email, Voice |

## Key Challenges
- **Transaction integrity:** State machine with strict transitions and rollback on failure at every step
- **RAG copilot:** Pinecone vector search over platform knowledge base for context-aware AI responses
- **Omni-channel inbox:** Unified message threading across 4 communication channels in a single UI
