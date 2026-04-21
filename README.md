# 🖨️ Print Management System

A university-focused web application designed to replace PaperCut with a cost-effective, internally managed printing solution. The system provides secure pull printing, quota control, device and queue management, comprehensive auditability, and admin visibility across the entire print workflow.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Project Motivation](#project-motivation)
- [System Architecture](#system-architecture)
- [System Users & Roles](#system-users--roles)
- [Core Use Cases](#core-use-cases)
- [Front-End Implementation](#front-end-implementation)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Setup & Installation](#setup--installation)
- [Running Locally](#running-locally)
- [Available Routes](#available-routes)
- [Team Members](#team-members)
- [Project Status](#project-status)
- [Documentation References](#documentation-references)
- [Important Notes](#important-notes)

---

## 📖 Project Overview

The Print Management System is a multi-phase initiative designed to modernize university printing infrastructure. Currently spanning **Phase 1** through **Phase 3**, the project progresses from initial concept through system design to a functional front-end prototype.

### Key Objectives

✅ Eliminate recurring PaperCut licensing costs  
✅ Provide full institutional control over printing infrastructure  
✅ Improve visibility into printing usage and associated costs  
✅ Deliver advanced analytics and reporting capabilities  
✅ Implement secure pull printing with quota-based access control  
✅ Enable comprehensive system auditability and logging  

---

## 🎯 Project Motivation

### Why Replace PaperCut?

The existing PaperCut printing solution requires:

- **Recurring licensing fees** that burden the institution's budget
- **Limited customization** to meet specific university needs
- **Restricted visibility** into detailed printing usage patterns and costs
- **Vendor dependency** for updates, support, and feature requests

### Our Solution

By building an **internally managed alternative**, we gain:

- **Cost Efficiency**: Eliminate licensing costs and optimize resource allocation
- **Full Control**: Customize workflows and policies to match institutional requirements
- **Transparency**: Real-time visibility into printing usage, costs, and trends
- **Scalability**: Design the system to grow with institutional needs
- **Analytics**: Comprehensive reporting on print jobs, user behavior, and cost analysis

---

## 🏗️ System Architecture

### 📊 System Diagrams

The complete system architecture is documented in **Phase 2**, including:

- **System Context Diagram** - High-level system boundaries and external interfaces
- **Use Case Diagram** - Visual representation of all user interactions
- **Entity-Relationship Models** - Database schema and data relationships
- **System Sequence Diagrams** - Detailed interaction flows

### 📄 Design Documentation

- **SRS Document**: [Print Management System SRS](https://github.com/user-attachments/files/25399996/Print.Manamgement.System.SRS.Doc.pdf)
- **UI/UX Prototype**: [Figma Design File](https://www.figma.com/files/team/1369054191536550891/project/230760201?fuid=1369054189176563017)

---

## 👥 System Users & Roles

The system is designed with three primary user roles, each with specific capabilities:

### 1️⃣ Administrator (Admin)

Full system control and oversight responsibilities.

**Capabilities:**
- Manage printing devices and print queues
- Modify user print quotas and access permissions
- Manage user and group access control
- View logs and comprehensive analytics dashboard
- Monitor cost calculations and billing
- Receive critical system alerts

### 2️⃣ Technician

Operational support and user assistance role.

**Capabilities:**
- Modify user print quotas
- Manage user and group access
- Receive system error notifications and alerts
- Monitor operational issues and device status
- Assist with user troubleshooting

### 3️⃣ Standard User

End-user printing interface.

**Capabilities:**
- Submit print jobs to available printers
- View personal printing history and quota usage
- Receive notifications on job status
- Access printing analytics for personal usage

---

## 📌 Core Use Cases

| Use Case ID | Title | Actor | Purpose |
|---|---|---|---|
| UC-01 | Request Print Job | Standard User | Submit a new print job for processing |
| UC-02 | View Printing History | Standard User | Access personal printing records and statistics |
| UC-03 | Manage Printing Devices | Admin | Configure, enable/disable, and monitor printers |
| UC-04 | Manage Printing Queues | Admin | Manage print queues and job prioritization |
| UC-05 | Modify User Quota | Admin/Technician | Adjust print quotas and access limits |
| UC-06 | Manage User Access | Admin/Technician | Control user and group permissions |
| UC-07 | View Logs & Analytics | Admin | Access system logs and generate reports |
| UC-08 | Receive Error Notifications | Admin/Technician | Get alerts on system errors and issues |

### ⚙️ Key Functional Areas

**Authentication & Authorization**
- Single Sign-On (SSO) integration with institutional directory
- Role-based access control (RBAC)
- Secure session management

**Print Job Management**
- Job submission and queuing
- Document processing and format handling
- Print job tracking and status monitoring
- Job cancellation and reprinting

**Print History & Analytics**
- User print history tracking
- Cost per print calculation
- Usage analytics and trends
- Quota enforcement and warnings

**Device & Queue Management**
- Printer device configuration
- Print queue creation and management
- Device status monitoring
- Print queue optimization

**User & Quota Management**
- User and group management
- Quota assignment and modification
- Access control enforcement
- Quota alerts and notifications

**Logging & Auditing**
- Comprehensive system audit logging
- User action tracking
- Print job audit trails
- System event logging

**Cost Calculation**
- Per-page cost calculation
- Color vs. black & white pricing
- Quota-based billing
- Cost analytics and reporting

**Error Detection & Notifications**
- Real-time error detection
- Error notifications to admin/technician
- Error logging and tracking
- System health monitoring

---

## 💻 Front-End Implementation

### Phase 3 Overview

The current Phase 3 delivers a **functional React prototype** demonstrating the complete user interface for all three user roles. The prototype uses **mock data** to simulate system behavior while backend integration is prepared separately.

### Front-End Scope

The prototype includes comprehensive UI screens for:

**Standard User Portal**
- Dashboard with print quota overview
- Print job submission form
- Printing history with filters and sorting
- Job status tracking

**Admin Dashboard & Management**
- System overview and key metrics
- User and group management
- Printer device management
- Print queue configuration
- Device status monitoring
- Reports and analytics
- System settings and options
- Audit logs viewer
- System information page

**Technician Dashboard**
- Quick access to key metrics
- User management for support
- Printer monitoring
- System alert notifications

**Interactive Features**
- Responsive layouts for desktop and tablet views
- Form validation and error handling
- Real-time status indicators
- Comprehensive data tables with sorting/filtering
- Modal dialogs for detailed operations
- Toast notifications for user feedback

---

## 🛠️ Tech Stack

### Frontend Stack

| Technology | Purpose | Version |
|---|---|---|
| **React** | UI framework | 18+ |
| **TypeScript** | Type-safe JavaScript | 5+ |
| **Vite** | Build tool & dev server | 5+ |
| **Tailwind CSS** | Utility-first CSS framework | 3+ |
| **React Router** | Client-side routing | 6+ |
| **Radix UI** | Headless UI primitives | Latest |

### Development Tools

- **npm** 10+ for package management
- **Node.js** 20+ runtime

### Backend (Planned)

- RESTful API for frontend communication
- Active Directory/SSO integration
- Database layer for persistence
- Embedded device communication

---
