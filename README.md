# National Blood Availability Intelligence

> **Smart India Hackathon 2026 — Software Solution**  
> **Team SynapTech**

## Overview

**National Blood Availability Intelligence** is an intelligent,
connected blood-bank network designed to improve emergency blood
fulfillment.

Instead of relying on manual coordination between individual blood
banks, the proposed system connects multiple blood banks and dynamically
evaluates available inventory to recommend the best way to fulfill
critical hospital requests.

The system can split an emergency requirement across multiple blood
banks when a single bank cannot fulfill the complete request.

### Example

A hospital urgently requests **3 units of O-negative blood**.

The system can:

1.  Scan connected blood banks in real time.
2.  Evaluate blood compatibility, quantity, distance, expiry urgency,
    and transport time.
3.  Recommend a split such as:
    - Blood Bank B → 2 units
    - Blood Bank C → 1 unit
4.  Present the recommendation to the dispatcher through a real-time
    dashboard.

## Key Features

- Real-time blood inventory synchronization across connected blood banks
- Emergency blood request broadcasting
- Blood compatibility evaluation
- Multi-bank inventory aggregation
- Intelligent split-fulfillment recommendations
- Distance and transport-time evaluation
- Expiry-aware inventory prioritization
- Real-time dispatcher dashboard
- Geospatial blood-bank search
- Scalable architecture for city, state, and larger blood-bank networks

## Proposed Technology Stack

### Frontend

- React.js
- Tailwind CSS

### Backend & Logic

- Node.js
- Python
- FastAPI

### Database & Geospatial

- PostgreSQL
- PostGIS

### Maps & Routing

- Mapbox
- OSRM

### Real-Time & Messaging

- Webhooks
- Redis

### Architecture

- Cloud microservices
- Geospatial routing services
- Integration with hospital management systems and courier networks

## System Workflow

``` text
Hospital Emergency Request
            |
            v
   Emergency Broadcast
            |
            v
Connected Blood Banks
            |
            v
Inventory & Compatibility Check
            |
            v
Multi-Factor Evaluation
            |
     +------+------+
     |             |
 Quantity       Distance
     |             |
 Expiry        Transport Time
     +------+------+
            |
            v
Split-Fulfillment Recommendation
            |
            v
 Dispatcher Dashboard
```

## Multi-Factor Evaluation

The recommendation engine evaluates:

- **Compatibility** — suitability of available blood for the requested
  blood type
- **Quantity** — available units at each blood bank
- **Distance** — geographic proximity to the requesting hospital
- **Expiry** — urgency of units approaching expiry
- **Transport Time** — estimated delivery time

## Proposed Process

### 1. Inventory Synchronization

Connected blood banks synchronize inventory through real-time webhooks.

### 2. Emergency Request

A hospital submits the blood type, required unit count, and hospital
coordinates.

### 3. Evaluation

The system evaluates available inventory using compatibility, distance,
expiry urgency, stock availability, and transport information.

### 4. Recommendation

The system generates an instant multi-bank fulfillment recommendation
for dispatchers.

## Feasibility & Scalability

The proposed architecture uses cloud microservices and standard
geospatial routing libraries.

The system is intended to:

- Integrate with existing hospital management systems
- Work with courier networks
- Scale from city-level clusters to statewide blood grids
- Minimize training requirements through a simple dispatcher interface

For crisis-related network latency, the proposed architecture includes
distributed edge caching and Redis messaging queues.

## Expected Impact

### Healthcare

- Reduce delays for critical and rare blood-type requirements
- Improve emergency blood availability visibility
- Support faster emergency fulfillment

### Blood Banks

- Reduce manual inter-bank coordination
- Improve utilization of available inventory
- Enable dynamic redistribution of near-expiry units

### Emergency Responders

- Provide a single-window view of available resources
- Support automated dispatch routing

### Environmental

Optimized multi-stop delivery routes can help reduce unnecessary travel,
fuel consumption, and emissions.

## Research & References

The proposed solution considers:

- **e-RaktKosh standards** for blood-bank inventory management
- **National Blood Transfusion Council (NBTC)** protocols related to
  cold-chain transport and cross-matching compliance
- Research on **multi-objective vehicle routing (MO-VRP)** for emergency
  medical supply chains

## Project Status

This repository represents the **Smart India Hackathon 2026 project and
proposed prototype architecture** for National Blood Availability
Intelligence.

> Technology listed in this README reflects the proposed technical
> approach in the SIH 2026 submission. Individual components should be
> marked as implemented only after they are actually developed and
> integrated.

## Team

**Team SynapTech**

- Ayushi Maheshwari
- Yash Vardhan Bansal
- Vinayak Puri
- Kushagra Pandey
- Chitansh Aggrawal
- Aryan Chaudhary

## Smart India Hackathon

**Problem Statement:** National Blood Availability Intelligence  
**Category:** Software Solutions  
**Hackathon:** Smart India Hackathon 2026

------------------------------------------------------------------------

**Team SynapTech \| National Blood Availability Intelligence**
