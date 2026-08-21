# Tech Stack — National Blood Availability Intelligence
**Team SynapTech | SIH 2026 | Software Solutions (Healthcare & MedTech)**

## Frontend
- **React.js** — real-time dispatch dashboard UI
- **Tailwind CSS** — styling

## Backend
- **Node.js** — core backend services
- **Python (FastAPI)** — routing algorithm engine

## Database
- **PostgreSQL** — primary relational database
- **PostGIS** — geospatial extension for radius queries & distance matrix calculations

## APIs / External Services
- **Mapbox / OSRM** — live transport time estimation & routing

## Caching / Messaging
- **Redis** — distributed edge caching + messaging queues (handles network latency during high-load emergency scenarios)

## Infrastructure
- **Cloud microservices architecture**
- Integrates with existing **HMIS** (Hospital Management Information Systems) and courier network APIs

---

## Suggested Repo Structure
```
national-blood-availability-intelligence/
├── frontend/          # React + Tailwind
├── backend/
│   ├── node-service/  # Node.js services
│   └── fastapi-service/  # Python FastAPI routing engine
├── db/                # PostgreSQL/PostGIS schema & migrations
├── docs/
└── README.md
```

## Core Modules to Build
1. **Inventory Sync** — real-time webhook sync across connected blood banks
2. **Emergency Broadcast** — trigger with blood type, unit count, hospital coordinates
3. **Scoring Engine** — evaluates distance, expiry urgency, stock availability
4. **Split-Fulfillment Recommender** — instant multi-bank recommendation output

---
*Source: SIH 2026 Idea Submission Deck, Slide 3 (Technical Approach)*
