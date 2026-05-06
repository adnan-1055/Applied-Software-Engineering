# hk.net Knowledge Management System

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![Draw.io](https://img.shields.io/badge/Draw.io-F08705?style=for-the-badge&logo=diagrams.net&logoColor=white)

> A software design and implementation project demonstrating core principles of Applied Software Engineering — developed as part of UWL CS AY2025-26.

---

## Overview

The hk.net KMS enables authorised users to efficiently search and retrieve archived project emails, view metadata, download attachments, and subscribe to project updates. The design follows a strict modular architecture to ensure scalability and ease of maintenance.

---

## Key Features

| Feature | Description |
|---|---|
| 📐 UML Modelling | Use Case, Class, Sequence, and Component diagrams |
| 🔁 Design Patterns | Observer Pattern (notifications) + Facade Pattern (system control) |
| 📏 Business Logic | Enforced via OCL — invariants, preconditions, postconditions |
| 🧪 Automated Testing | JUnit 5 unit tests validating system constraints |
| ⚠️ Risk Management | Detailed risk register covering data quality, performance, and security |

---

## Architecture

The system is decomposed into specialised service layers following separation of concerns:

```
┌─────────────────────────────────────────┐
│              Facade Layer               │
└────────────┬────────────────────────────┘
             │
    ┌────────▼─────────┐
    │   AuthService    │  → User credentials & access control
    │  ProjectService  │  → Project data & subscriptions
    │  EmailService    │  → Filtered search & retrieval
    │AttachmentService │  → Secure file downloads
    │  StorageService  │  → Exports for auditing & portability
    └──────────────────┘
```

---

## Project Structure

```
hk-net-kms/
├── src/
│   └── ...          # Java source — domain model & service logic
├── tests/
│   └── ...          # JUnit 5 tests validating OCL constraints
└── docs/
    └── ...          # UML diagrams & risk analysis
```

---

## Technologies Used

- **Java** — backend implementation using OOP principles
- **JUnit 5** — unit testing and constraint verification
- **Draw.io** — UML modelling
- **Maven** — dependency and build management

---

*Developed by Mohammed Adnan — Applied Software Engineering, University of West London*
