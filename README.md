<h1 align="center">
  <br>
  TenantsBook
  <br>
</h1>

<h4 align="center">A comprehensive Full-Stack SaaS platform for modern property management.</h4>

<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#key-features">Key Features</a> •
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#architecture">Architecture</a> •
  <a href="#screenshots">Screenshots</a>
</p>

---

## 🔗 Live Demo
**Website:** [https://tenantsbook.in/](https://tenantsbook.in/)

*(Note: If testing, please be respectful of the demo environment.)*

## Overview

**TenantsBook** is a professional, end-to-end property management system designed to streamline the rental experience for both landlords and tenants. Built with a focus on scalable backend architecture, it replaces scattered spreadsheets with a centralized, multi-tenant ecosystem for lease tracking, automated financial invoicing, and stateful maintenance management.

> **Note:** This repository is a public showcase / demo repository. The source code for the proprietary backend and frontend is maintained in private repositories. 

## Key Features

- **Multi-Tenant Architecture:** Secure role-based access control (RBAC) isolating Landlord and Tenant contexts via strict Entity Framework query filters and Row-Level Security principles.
- **Automated Financial Engine:** Background logic dynamically evaluates lease parameters (lock-in periods, notice periods) to generate automated monthly Rent Invoices and calculate dynamic late fees.
- **Dynamic Document Generation:** Service-layer generation of legally-structured, professional Lease Agreements and Rent Invoices rendered directly to memory streams.
- **Stateful Ticket Management:** Robust state machine for maintenance requests, enforcing valid entity state transitions (Open → Assigned → Closed) across secure endpoints.
- **High-Performance Analytics:** Dashboard metrics powered by conditional SQL aggregation and caching, drastically minimizing database round-trips for real-time data visualization.
- **Secure Cloud Storage:** Decoupled document management service integrating secure file streaming for KYC proofs, signed leases, and property assets.

## Tech Stack

### Backend
- **Framework:** .NET 10 Web API (C#)
- **Architecture:** Clean Architecture, Interface-based Dependency Inversion, Repository Pattern
- **ORM:** Entity Framework Core (Code-First)
- **Database:** PostgreSQL (with Npgsql)
- **Integrations:** Brevo API (Transactional Emails), Supabase Auth (JWKS-based JWT validation)

### Frontend
- **Framework:** React 19 + Vite
- **Language:** TypeScript
- **State & UI:** Modern React Patterns, Custom UI components, and Responsive Design
- **Hosting:** Cloudflare Pages

## Architecture
Curious about how the backend is structured? Read the detailed [Architecture Documentation](./ARCHITECTURE.md) covering Dependency Injection, Domain-Driven Error Handling, our Notification Engine, and custom cross-region Performance Mitigations.

---

## Screenshots

<details>
<summary><b>Click to expand and view application screenshots</b></summary>
<br>

*(Note: Below are a few select screens from the application)*

### Landlord Dashboard
![Dashboard](assets/screenshots/tenantBook-screen1.png)

### Properties Overview
![Properties](assets/screenshots/tenantBook-screen2.png)

### Unit Details
![Unit Details](assets/screenshots/tenantBook-screen3.png)

### Lease Management
![Lease Management](assets/screenshots/tenantBook-screen4.png)

### Automated Invoicing
![Invoicing](assets/screenshots/tenantBook-screen5.png)

### Maintenance Tickets
![Maintenance](assets/screenshots/tenantBook-screen6.png)

</details>

---

## Contact
**Developer:** Shawez  
**Email:** shawez.dev@gmail.com  
**LinkedIn / GitHub:** Feel free to reach out via email for access to the complete source code or to discuss the backend system design in depth!

<p align="center">
  <i>Engineered with ❤️ for modern property management.</i>
</p>
