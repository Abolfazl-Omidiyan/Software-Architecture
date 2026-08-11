# Low-Code Inspired BPMS Architecture

## Overview

This project was developed as a final project for the Software Architecture course.

The project investigates the architectural aspects of Low-Code and No-Code platforms through the design and implementation of an executable Business Process Management System (BPMS). Rather than focusing on rapid application development, the project analyzes how architectural decisions, workflow execution, component interaction, and layered structures are realized in a BPMS environment.

The implemented system manages organizational request workflows and demonstrates how a workflow engine can be integrated within a layered software architecture.

---

## Project Objectives

- Study the architectural foundations of Low-Code / No-Code platforms
- Analyze architectural patterns used in modern workflow systems
- Design an executable software architecture
- Implement a BPMS prototype
- Model software architecture using UML and BPMN
- Evaluate architectural quality attributes

---

## Research Topic

**Software Architecture in Low-Code and No-Code Platforms: Architectural Analysis, Benefits, and Challenges**

The project investigates:

- Model-Driven Architecture (MDA)
- Service-Oriented Architecture (SOA)
- API-Driven Architecture
- Workflow Engines
- Layered Architecture
- Architectural Quality Attributes
- Architectural Trade-offs
- Vendor Lock-In Challenges

---

## Architecture Overview

The system follows a Layered Architecture pattern.

```text
Presentation Layer
        │
        ▼
API Layer
        │
        ▼
Business Layer
        │
        ▼
Persistence Layer
        │
        ▼
Data Layer
```

### Layers

#### Presentation Layer
- HTML
- CSS
- Bootstrap
- JavaScript

#### API Layer
- Flask REST API
- Controllers

#### Business Layer
- Workflow Engine
- Approval Service
- Business Rules
- Notification Service

#### Persistence Layer
- Repositories
- SQLAlchemy ORM

#### Data Layer
- MySQL Database

---

## Implemented Architectural Views

The project includes the following architectural models:

### Use Case Diagram
Actors:
- Employee
- Manager
- HR Officer
- System Administrator

### Layered Architecture Diagram
Defines the logical separation of responsibilities.

### Component Diagram
Main Components:
- Web Frontend
- Request Controller
- Workflow Controller
- Authentication Service
- Workflow Service
- Notification Service
- Repositories
- Database

### BPMN Workflow Diagram

Workflow:

Request Submission
→ Manager Review
→ Approval Decision
→ HR Approval
→ Notification
→ Workflow Completion

### Deployment Diagram

Browser
→ Flask Application Server
→ MySQL Database

---

## Business Process Workflow

```text
Start
  │
  ▼
Submit Request
  │
  ▼
Manager Review
  │
  ▼
Approved?
 ├── No → Reject Request → End
 └── Yes
         │
         ▼
    HR Review
         │
         ▼
    Final Approval
         │
         ▼
    Close Workflow
         │
         ▼
        End
```

---

## Technology Stack

### Backend
- Python
- Flask
- SQLAlchemy

### Frontend
- HTML5
- CSS3
- Bootstrap
- JavaScript

### Database
- MySQL

### Modeling Tools
- Sparx Enterprise Architect
- BPMN 2.0
- UML

---

## Quality Attributes Analysis

### Maintainability
Layer separation improves maintainability and code organization.

### Modifiability
Workflow rules can be extended with minimal impact on other layers.

### Scalability
REST-based architecture allows future horizontal scaling.

### Security
Authentication and authorization are isolated in dedicated components.

### Interoperability
External APIs can be integrated through the API Layer.

---

## Project Structure

```text
bpms-project/
│
├── frontend/
│
├── backend/
│
├── architecture/
│   ├── use-case-diagrams/
│   ├── layered-architecture/
│   ├── component-diagrams/
│   ├── bpmn-models/
│   └── deployment-diagrams/
│
├── docs/
│
├── presentation/
│
└── README.md
```

---

## Project Deliverables

- Research Report
- Architecture Analysis Report
- UML Models
- BPMN Models
- Executable Architecture
- GitHub Repository
- Technical Presentation
- Video Demonstration

---

## Article

Project article published on Virgool:

https://vrgl.ir/PzYDG

---

## Video Presentation

Project presentation video:

https://aparat.com/v/ytc963b

---

## References

- Bass, L., Clements, P., Kazman, R. *Software Architecture in Practice*
- Kruchten, P. *The 4+1 View Model of Architecture*
- BPMN 2.0 Specification
- Microsoft Power Platform Architecture Documentation
- Mendix Architecture Documentation
- OutSystems Architecture Documentation
- IEEE and ACM Research Papers on Low-Code Architectures

---

## Author
Abolfazl Omidiyan

Software Architecture Course Project

Master of Information Technology (IT)

Enterprise Architecture & Intelligent Systems Research
