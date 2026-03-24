# NAMMA TRICHY

### Unified Mobility and City Experience Platform for Tiruchirappalli

---

## Overview

ONE TRICHY is a full-stack web application designed to unify urban mobility and city exploration into a single, cohesive platform. Inspired by modern multimodal transport systems, it integrates route planning, ticketing, mapping, and immersive city discovery into one interface.

The platform combines transport infrastructure with a cinematic user experience, delivering both functionality and visual depth.

---

## Key Features

### 1. Multimodal Journey Planning

* Plan routes across:

  * Public buses
  * Trains
  * Private transport (auto/taxi)
* Displays:

  * Estimated travel time
  * Cost breakdown
  * Transfer points

### 2. Interactive Map Integration

* Built using Leaflet.js
* Real-time simulated vehicle movement
* Route visualization using polylines
* Clickable markers with contextual data

### 3. Unified Ticketing System

* Book tickets across transport modes
* QR-based ticket generation
* Ticket history and tracking
* Structured booking workflow

### 4. Private Transport Booking

* Select ride type (auto, cab, etc.)
* Dynamic fare estimation
* Location-based booking interface

### 5. Public Transport Module

* Bus/train search and filtering
* Seat availability simulation
* Multi-step booking and confirmation flow

### 6. Explore Tiruchirappalli

* Cinematic carousel interface
* Dynamic background transitions
* Location-based storytelling
* Navigation integration with transport system

### 7. High-End UI/UX System

* Dark, cinematic design language
* Typography:

  * Anton (headings)
  * EB Garamond (body)
* Smooth transitions and animations
* Fully responsive layout

---

## Tech Stack

### Frontend

* HTML5 / CSS3
* JavaScript (Vanilla)
* Tailwind-inspired custom styling
* Leaflet.js (maps)

### Backend (Planned / Extendable)

* Node.js (Express)
* REST API architecture

### Database

* PostgreSQL

---

## Project Structure

```
/client
  ├── index.html
  ├── explore.html
  ├── public-transportation-tickets.html
  ├── private-transportation.html
  ├── assets/
  │    ├── images/
  │    └── styles/

/server (planned)
  ├── server.js
  ├── routes/
  ├── controllers/

/database
  ├── schema.sql
```

---

## Installation and Setup

### Prerequisites

* Node.js (v18+)
* PostgreSQL
* npm

---

### 1. Clone Repository

```
git clone https://github.com/your-username/one-trichy.git
cd one-trichy
```

---

### 2. Frontend Setup

```
cd client
npm install
npm run dev
```

---

### 3. PostgreSQL Setup

Create database:

```
createdb one_trichy
```

Run schema:

```
psql -d one_trichy -f database/schema.sql
```

---

### 4. Backend Setup (if implemented)

```
cd server
npm install
node server.js
```

---

## Database Schema (Core Tables)

```
Users(id, name, email, password_hash)

Routes(id, source, destination, type)

Vehicles(id, route_id, type, current_location)

Tickets(id, user_id, route_id, qr_code, status)

Passes(id, user_id, type, valid_until)

Transactions(id, user_id, amount, status)
```

---

## Design Philosophy

The platform is built on three core principles:

1. **Unified Experience**
   Transport and city exploration are not separate systems.

2. **Clarity over Complexity**
   Minimal UI with high usability.

3. **Immersive Interaction**
   Cinematic visuals combined with real functionality.

---

## Future Enhancements

* Real-time GPS integration
* AI-based route optimization
* Progressive Web App (PWA)
* Multilingual support (Tamil + English)
* Payment gateway integration (UPI)
* Admin dashboard for transport management

---

## Use Cases

* Urban commuters
* Tourists exploring Tiruchirappalli
* Smart city infrastructure prototypes
* Academic and hackathon projects

---

## License

MIT License

---

## Author

Kumaran Chandrashekar
Computer Science (Data Science)
VIT Chennai
