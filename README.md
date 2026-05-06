hk.net Knowledge Management System (KMS)
This repository contains the software design and implementation of the hk.net Knowledge Management System, a project developed to demonstrate core principles of Applied Software Engineering.

Overview
The system enables authorized users to efficiently search and retrieve archived project emails, view metadata, download attachments, and subscribe to project updates. The design follows a strict modular approach to ensure scalability and ease of maintenance.

Key Features
Comprehensive UML Modelling: Includes Use Case, Class, Sequence, and Component diagrams.

Design Patterns: Implementation of the Observer Pattern to manage notifications and the Facade Pattern to centralize system control.

Robust Business Logic: Enforced using Object Constraint Language (OCL) to manage invariants, preconditions, and postconditions.

Automated Testing: Unit testing with JUnit 5 to validate system constraints and business rules.

Risk Management: A detailed risk register addressing data quality, performance, and security.

Architecture
The system is decomposed into specialized service layers to promote separation of concerns:

AuthService: Handles user credentials and access control.

ProjectService: Manages project data and subscriptions.

EmailService: Executes filtered searches and retrieves email details.

AttachmentService: Facilitates secure file downloads.

StorageService: Handles exports for auditing or portability.

Project Structure
src/: Java source code implementing the domain model and service logic.

tests/: Unit tests validating invariants and OCL constraints.

docs/: Design artifacts including UML diagrams and risk analysis.

Technologies Used
Java: Backend implementation using object-oriented principles.

JUnit 5: Unit testing and verification.

Draw.io: UML modelling tool.

Maven: Dependency and build management.
