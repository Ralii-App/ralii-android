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
- **RL-100** — Authentication & User Profiles
- **RL-200** — Community Jobs & Volunteering
- **RL-300** — Group Join Requests & Communication Links
- **RL-400** — Fundraisers & Donations
- **RL-500** — Discovery & Location Services
- **RL-600** — Trust, Safety & Moderation (planned)

This structure supports long-term growth and makes it easy for contributors to work on isolated features.

---

## 🛠 Tech Stack

- Kotlin
- Jetpack Compose
- Android Architecture Components
- REST API / Firebase (TBC)
- Modular Gradle setup

---


## 🔗 Related Repositories

- **Ralii Android App**  
  👉 https://github.com/Ralii-App/ralii-api

## 📂 Project Structure (Simplified)

