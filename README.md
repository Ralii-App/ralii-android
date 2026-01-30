# Ralii — Android App

Ralii is an open-source Android application that helps people discover nearby charities, volunteer opportunities, community jobs, and local fundraisers. The goal is to make it easy for individuals to take action in their communities — whether by volunteering time, donating items, or supporting local causes.

This repository contains the **Android client application**, built with scalability, modularity, and community contribution in mind.

---

## 🌍 What Ralii Does

With Ralii, users can:
- Find nearby charities and community initiatives
- Volunteer for local community jobs (e.g. clean-ups, repairs, outreach)
- Create and join grassroots community actions
- View and support fundraisers (monetary or item-based)
- Request to join charity-managed groups (WhatsApp, Discord, Instagram, email)

Ralii does **not** host chats or process payments directly — it connects people to existing platforms and trusted organisations.

---

## 🧱 Modular Architecture

The app is organised into clearly defined feature modules, inspired by university-style course codes. Each module owns its UI, logic, and data concerns.

### Core Modules
# 🔐 RL-100 — Identity & Access
Handles authentication, user identity, and role-based access.

**RL-101: User Authentication**
*   Sign up / sign in
*   Token validation (Firebase Auth / JWT)

**RL-102: User Profiles**
*   Personal details
*   Skills and interests

**RL-103: Roles & Permissions**
*   Volunteer
*   Charity / Organisation
*   Admin (future)

**Example Tables**
*   `rl101_users`
*   `rl103_user_roles`

---

# 🤝 RL-200 — Community Jobs
Supports the creation and participation of local, community-driven jobs.

**RL-201: Create Community Job**
*   Job details (title, description, category)
*   Location and time

**RL-202: Browse & Join Jobs**
*   View nearby jobs
*   Join or leave a job

**RL-203: Participation Tracking**
*   Track volunteers per job
*   Basic status management

**Example Tables**
*   `rl201_community_jobs`
*   `rl203_job_participants`

---

# 💬 RL-300 — Group Join Requests & Communication
Routes volunteers to charity-managed communication channels without hosting chats.

**RL-301: Charity Contact Channels**
*   WhatsApp
*   Discord
*   Instagram
*   Email

**RL-302: Join Requests**
*   "Request to join" submissions
*   Message templates

**RL-303: Join Request History (optional)**
*   Audit trail for charities

**Example Tables**
*   `rl301_charity_contacts`
*   `rl302_join_requests`

---

# 💰 RL-400 — Fundraisers & Donations
Manages fundraising initiatives while keeping financial transactions outside the platform.

**RL-401: Create Fundraiser**
*   Cause description
*   Goals and deadlines

**RL-402: Monetary Donations (Informational)**
*   Bank details
*   QR code data

**RL-403: Item-Based Donations**
*   Food, blankets, clothing, pet supplies

**RL-404: Fundraiser Status & Updates**

**Example Tables**
*   `rl401_fundraisers`
*   `rl403_donation_items`

> **Note:** The API does not process payments directly.

---

# 📍 RL-500 — Discovery & Location
Supports location-aware discovery of charities, jobs, and fundraisers.

**RL-501: Location Services**
*   Coordinates and regions

**RL-502: Nearby Search**
*   Radius-based queries

**RL-503: Filters & Categories**

**Example Tables**
*   `rl501_locations`
*   `rl502_entity_locations`

---

# 🛡️ RL-600 — Trust, Safety & Moderation (Planned)
Ensures platform integrity and user safety as the project grows.

**RL-601: Reporting**
*   Flag inappropriate content

**RL-602: Verification**
*   Trusted charities

**RL-603: Moderation Tools**

**Example Tables**
*   `rl601_reports`
*   `rl602_verification_status`

This structure supports long-term growth and makes it easy for contributors to work on isolated features.

---

## 🛠 Tech Stack

- Kotlin
- Jetpack Compose
- Android Architecture Components
- REST API / Firebase (TBC)
- Modular Gradle setup

---

## 📂 Project Structure (Simplified)

