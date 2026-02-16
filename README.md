# 🚀 CodeOne — Consolidate Your Competitive Programming Journey  

> The unified analytics layer for competitive programmers.  
> Track. Analyse. Improve. Stay consistent.

![Node](https://img.shields.io/badge/Node.js-18+-green)
![React](https://img.shields.io/badge/React-18+-blue)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Status](https://img.shields.io/badge/Status-Production--Ready-success)

---

## 📌 Table of Contents

- [✨ Overview](#-overview)
- [🚀 Why CodeOne?](#-why-codeone)
- [🔥 Core Features](#-core-features)
- [🛠 Tech Stack](#-tech-stack)
- [🏗 Architecture](#-architecture)
- [🔐 Authentication](#-authentication)
- [🗄 Database Schema](#-database-schema)
- [🔌 API Design](#-api-design)
- [🌍 Environment Variables](#-environment-variables)
- [⚙ Local Setup](#-local-setup)
- [📁 Project Structure](#-project-structure)
- [🚀 Deployment](#-deployment)
- [📊 Design Decisions](#-design-decisions)
- [🛣 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [📬 Contact](#-contact)

---

## ✨ Overview

**CodeOne** is a full-stack competitive programming analytics platform built for developers, students, and interview aspirants solving problems across:

- LeetCode  
- Codeforces  
- HackerRank  
- AtCoder  
- CodeChef  

Instead of switching between multiple dashboards, CodeOne provides a **single intelligent control center** for:

- 📊 Progress tracking  
- 🔥 Streak monitoring  
- 📈 Difficulty analysis  
- 🧠 Topic mastery  
- 🏆 Contest planning  

---

## 🚀 Why CodeOne?

Competitive programmers often struggle with:

- ❌ Fragmented progress tracking  
- ❌ No unified analytics  
- ❌ Lack of streak visibility  
- ❌ Poor long-term performance insights  

CodeOne solves this by acting as a **performance intelligence layer** on top of existing platforms.

It’s not just a tracker.  
It’s a **consistency engine**.

---

## 🔥 Core Features

### 📊 Unified Analytics Dashboard
- Daily activity heatmap
- Global streak tracker
- Platform comparison metrics
- Difficulty distribution chart
- Submission trends graph

### 🧠 Smart Problem Management
- Filter by platform, tags, difficulty
- Status tracking (Solved / In Progress / Review Later)
- Topic-wise breakdown

### 🔥 Streak Intelligence
- Current & longest streak
- Year-long contribution heatmap
- Platform-wise streak comparison

### 🏆 Contest Intelligence
- Upcoming contest aggregation
- Countdown timers
- Direct registration links

### ⚙ Advanced Profile Management
- Platform account linking
- Goal tracking (Daily / Weekly)
- Notification preferences
- Dark mode support

---

## 🛠 Tech Stack

### Frontend
- ⚛ React.js (Vite)
- 🎨 Tailwind CSS
- 📊 Recharts
- 🔄 Axios

### Backend
- 🟢 Node.js
- 🚀 Express.js
- 🧩 Modular Service Architecture

### Database
- 🐘 PostgreSQL (Primary)
- ⚡ Redis (Caching & streak computation)

### DevOps & Tooling
- 🐳 Docker
- 🔐 JWT + OAuth
- ☁ Cloud Deployment Ready
- 📦 RESTful API Design

---

## 🏗 Architecture

**Architecture Type:** Modular Monolith (API-First)

### 🔷 High-Level Architecture

```mermaid
flowchart LR
    A[React Client] --> B[Express API Layer]
    B --> C[Auth Module]
    B --> D[Analytics Engine]
    B --> E[Contest Aggregator]
    C --> F[(PostgreSQL)]
    D --> F
    D --> G[(Redis Cache)]
    E --> F
