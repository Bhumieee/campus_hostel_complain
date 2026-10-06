# CampusFix - Smart Campus Infrastructure Management & Issue Tracking Platform

[![Status](https://img.shields.io/badge/Status-Hackathon_MVP-blue.svg)](https://github.com)
[![Stack](https://img.shields.io/badge/Stack-MERN_FullStack-green.svg)](https://github.com)
[![Architecture](https://img.shields.io/badge/Architecture-REST_API-orange.svg)](https://github.com)
[![Anonymity](https://img.shields.io/badge/Anonymity-Tokenized-purpe.svg)](https://github.com)



## Executive Summary
Colleges and university campuses frequently suffer from broken infrastructure (e.g., damaged lab equipment, faulty projector systems, broken plumbing, or malfunctioning air conditioners). Traditional complaint systems suffer from high friction, slow resolution times, lack of transparency, and poor accountability.

This platform streamlines campus maintenance through **QR-code based micro-reporting**, **crowdsourced issue prioritization**, and **transparent, photo-verified resolution loops**.

---

## Key Features & Solution Pillars

### 1. QR Code Asset Mapping
- Every institutional asset (desk, projector, lab equipment, washroom, AC unit) is tagged with a unique, tamper-evident QR code.
- Scanning the code instantly loads a contextual complaint form pre-populated with precise hardware and location metadata.

### 2. Low-Friction Anonymous Reporting
- Students and staff can log complaints without sign-in barriers or fear of administrative friction.
- Prevents redundant ticket creation by checking active reports bound to the scanned Asset ID.

### 3. Campus Live Feed & Crowd Prioritization
- All active non-sensitive complaints are published to a public campus dashboard.
- Students and faculty upvote existing issues to dynamically elevate high-impact problems to top priority.

### 4. Smart Technician Dispatch
- Tickets automatically trigger alerts for department-specific maintenance staff (IT, Electrical, Plumbing, Civil).
- SLA tracking monitors time-to-assignment and time-to-resolution.

### 5. Proof-of-Work & Student Verification Loop
- Technicians must upload a **photo proof of repair** to transition a ticket to "Pending Verification."
- The original reporter (or community upvoters) receives a notification to verify and close the ticket, closing the accountability loop.

---

## Technical Stack Architecture

| Layer | Technology Recommendations |
| :--- | :--- |
| **Frontend** | React / Next.js , Progressive Web App (PWA) |
| **Backend** | Node.js (Express/Fastify) or Python (FastAPI) |
| **Database** | PostgreSQL (Relational metadata) + Redis (Live feed caching & upvote counts) |
| **Storage** | Amazon S3 / Cloudflare R2 (Photo proof uploads & QR assets) |
| **Notifications**| Web Push Notifications / WhatsApp Webhooks / Email |
