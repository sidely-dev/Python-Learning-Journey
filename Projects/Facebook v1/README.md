# 🚀 SocialNet (Facebook v1 Clone)

> A full-stack, scalable social networking platform modeled after Facebook's original architecture, featuring user profiles, dynamic newsfeeds, relational friendship networks, media uploads, and real-time interaction loops.

<!-- Project badges -->
![Status](https://shields.io)
![Version](https://shields.io)
![Language](https://shields.io)
![License](https://shields.io)

---

## 📌 Table of Contents

- [About The Project](#-about-the-project)
- [Project Objectives](#-project-objectives)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [How It Works](#-how-it-works)
- [Getting Started](#-getting-started)
- [Installation](#-installation)
- [Usage](#-usage)
- [Bugs & Fixes](#-bugs--fixes)
- [Challenges & Struggles](#-challenges--struggles)
- [What I Learned](#-what-i-learned)
- [Development Process](#-development-process)
- [Roadmap](#-roadmap)
- [Known Issues](#-known-issues)
- [Future Improvements](#-future-improvements)
- [Project Reflection](#-project-reflection)
- [License](#-license)
- [Author](#-author)

---

## 📖 About The Project

### What is this project?

> This project is a robust, full-stack social connection ecosystem built with Python on the backend and modern reactive components on the frontend. It explores the foundational mechanics of early social spaces: the dynamic algorithmic Newsfeed, the interactive "Wall," friend management systems, and media sharing.

The core intent is to map how complex, multi-layered data objects (Users, Posts, Comments, Likes, and Friends) interact under strict relational schema rules while maintaining sub-second delivery timelines to clients.

### Why did I build it?

This project was created to master:
- **Relational Data Mapping:** Architecting complex Self-Referential Many-to-Many relationships (e.g., users adding other users as friends).
- **Feed Generation Algorithms:** Designing efficient database querying mechanics to pull, sort, and stitch together posts created exclusively by a user's friend list.
- **Secure Authentication Gates:** Setting up industrial-grade password encryption and secure cookie-based session management pipelines.
- **Media Ingestion Assets:** Connecting secure file upload channels to parse, compress, and store profile and post imagery.

### Project Background

This is a comprehensive full-stack portfolio capstone project built to understand how high-volume social platforms handle relational lookups, secure data privacy parameters, and fast asset streaming smoothly.

---

## 🎯 Project Objectives

The main objectives of this project are:

- [ ] Structure an authenticated, secure profile dashboard container for user custom walls.
- [ ] Implement an aggregated, reverse-chronological Newsfeed algorithm pulling multi-user post objects.
- [ ] Build a self-referential friend request transaction manager handling Pending, Accepted, and Blocked statuses.
- [ ] Connect cloud file attachment buckets to handle high-resolution image rendering streams safely.
- [ ] Deploy the complete live production platform onto isolated scalable cloud hosting environments.

---

## ✨ Features

### ✅ Implemented Features

- **The Interactive Wall Interface** — A responsive workspace layout featuring chronological personal posting lists, profile headers, and user detail cards.
- **Secure Authentication Gates** — Modern login and signup dashboard pages with server-side field input sanitation loops.
- **Granular Post System** — Capability to create, publish, and delete raw text status posts natively inside the timeline view.

### 🚧 Features Currently Being Developed

- **The Newsfeed Aggregator** — Writing highly optimized Python queries that scan a user's active friend database vector and return unified status feeds.
- **Friend Request Engine** — A dedicated internal logic structure handling friend invitations, approval prompts, and follower balance logs.
- **Interactive Response Deck** — Adding unified backend API endpoints to handle single-tap Likes and nested Comment creation arrays dynamically.

### 🔮 Planned Features

- [ ] **Real-Time Notification Core** — Integrating long-polling or WebSocket configurations to alert users instantly when their wall receives an interaction.
- [ ] **Global Search Autocomplete** — An efficient, text-indexing look-up engine that finds user profiles instantly via string matches.

---

## 🛠️ Technologies Used

| Layer | Technology | Purpose |
|---|---|---|
| **Backend Framework** | Python + Flask (or Django) | Directs corporate business rules, API routing paths, and database operations |
| **Database ORM** | PostgreSQL + SQLAlchemy | Handles relational database schemas for users, posts, and friendship matrices |
| **Frontend Deck** | HTML5, CSS3, JavaScript | Implements interactive dashboards, post forms, and responsive components |
| **Media Storage** | AWS S3 / Local Storage | Secure object storage layer hosting profile photos and timeline images |
| **Security Layer** | Passlib / bcrypt | Manages secure hashing of critical account credentials |
| **Version Control** | Git & GitHub | Manages workflow feature branch rollouts and snapshots |

### Languages

- Python (Backend API & Services)
- JavaScript (Client-side interactive behaviors)
- HTML5 & CSS3

### Frameworks / Libraries

- Flask / Django (Python Server Architectures)
- SQLAlchemy (Object Relational Model mapping)
- Jinja2 (Dynamic server-side page template compilation)

### Development Tools

- VS Code / PyCharm (IDE Workspace)
- Git & GitHub Actions
- PostgreSQL pgAdmin Suite (Database Inspection)

---

## 📂 Project Structure

```text
socialnet-facebook-clone/
│
├── app/
│   ├── templates/          # Jinja2 dynamic views (feed.html, profile.html, login.html)
│   ├── static/
│   │   ├── css/            # Classic clean multi-column layouts, newsfeed grids, and profile scales
│   │   └── js/             # Feeds interactive form listeners, asynchronous like counters
│   │
│   ├── models/             # Python Relational Database Schemas
│   │   ├── user.py         # Account details, password hash slots, and self-referential friend linkages
│   │   ├── post.py         # Text data properties, timeline markers, and user foreign key links
│   │   └── interaction.py  # Schemes organizing comment text trees and individual like counts
│   │
│   ├── routes/             # Core Backend REST API Handlers
│   │   ├── main.py         # Aggregates newsfeed collection logic and render sequences
│   │   ├── auth.py         # Security controllers protecting login actions and registration sessions
│   │   └── social.py       # Tracks friend adjustments, profile posts, and likes metrics
│   │
│   └── __init__.py         # Bundles core components and triggers database connection pools
│
├── docs/
│   └── screenshots/        # Application view captures presenting dashboard timelines
│
├── requirements.txt        # Comprehensive Python library tracking manifest
├── .env.example            # Environmental variable setup document blueprints
└── README.md
```

---

## 🧠 How It Works

The mechanical interaction lifecycle of a social update generation sequence follows an absolute structural loop:

```text
User Submits Post
        │
        ▼
 Backend Captures Data
   (Cleans & Sanitizes)
        │
        ▼
   Save to Postgres
  (Generates Post ID)
        │
        ▼
Friend Requests Feed
        │
        ▼
Newsfeed Query Triggers
(Pulls Friend ID list -> Scans posts -> Sorts by date)
        │
        ▼
 Jinja2 Compiles View
        │
        ▼
Client Receives Updates
 (Renders feed instantly)
```

---

## 🚀 Getting Started

Follow the simple deployment parameters listed below to host and inspect this full-stack Python application locally.

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com
   cd socialnet-facebook-clone
   ```

2. **Initialize a Python Virtual Environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Acquire project library requirements**
   ```bash
   pip install -r requirements.txt
   ```

4. **Establish Environmental Configurations**
   Create a live `.env` file within your root project directory layout:
   ```text
   FLASK_APP=app
   FLASK_ENV=development
   SECRET_KEY=your_session_encryption_passphrase
   DATABASE_URL=postgresql://username:password@localhost:5432/socialnet_db
   ```

### Usage

1. **Initialize the local database tables**
   ```bash
   python -c "from app import db; db.create_all()"
   ```
2. **Fire up the backend Python engine**
   ```bash
   flask run
   ```
3. Open `http://127.0.0.1:5000` inside your favorite web browser dashboard view. Create two distinct user test profiles, associate them as friends, and verify the algorithmic Newsfeed synchronization live!

---

## 🐛 Bugs & Fixes

- **Bug:** Querying newsfeeds for users with zero active friends crashed the main template rendering stack.
- **Fix:** Structured defensive baseline fallbacks inside the python controller that inject empty list values smoothly if friend checks resolve to zero elements.

---

## 💡 Challenges & Struggles

