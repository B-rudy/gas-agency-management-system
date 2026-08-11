# Gas Agency Management System (GasMS)

A Pega-based case management application built for a fictional gas agency (GAM), automating cylinder booking, connection transfers, and complaint handling for consumers and agency managers.

**Team:** Pega Challengers
- Akhil Abhiram P — Scrum Master
- Venkata Rupa Vardhan B
- Nakul Sri Sai G
- Hitesh Krishna M

**Product Owner:** Mr. SatyaVeer Soma

---

## Overview

GasMS automates the end-to-end gas cylinder booking lifecycle across three core case types — **Gas Booking**, **Connection Transfer**, and **Booking Complaints** — reducing manual work for both consumers and agency managers. Key features include:

- Consumer registration with Aadhar/LPG ID validation
- Dynamic subsidy-based pricing (₹75 for cylinders within a 12-unit annual subsidy limit, ₹150 beyond)
- Automated email notifications (registration, booking confirmation, transfer, complaints)
- Same-city and different-city connection transfer workflows
- Manager approval flows for registration, payment, and transfer requests
- Consumer feedback collection and agency performance reporting

## Application Structure

Built on Pega's standard **ECS (Enterprise Class Structure)** layer with Data, Work, and Integration classes covering:
- **Data objects:** Consumer, Distributor, Payment Details, Feedback, Complaints, Connection Transfer
- **Work (case types):** Gas Booking, Connection Transfer, Booking Complaints
- **Portals:** User Portal, Manager Portal
- **Access Groups:** GasMS:Users, GasMS:Authors, GasMS:Managers

See [`HLD_GAM_Pega_Challengers.pdf`](./HLD_GAM_Pega_Challengers.pdf) for the full high-level design, including case lifecycle diagrams, data flow diagrams, and data type definitions.

## My Contribution

I worked on the **Connection Transfer** case type, including:
- Defining properties and data types for the transfer flow
- Building the "Termination Voucher" generation section for different-city transfers
- Contributing to shared UI screens (login, registration, booking, payment, feedback) and data page configuration alongside the team

## Agile Process

The project was delivered across **4 sprints**, following Scrum practices:
- Sprint planning with backlog items mapped to Pega case lifecycle stages
- Daily scrum tracking and sprint retrospectives
- Impediment logs (10 impediments identified and resolved across sprints)
- Actionable improvements captured each sprint for continuous process refinement

See [`UAP_KLU_TCS02_Gas_Agency_Management.xlsx`](./UAP_KLU_TCS02_Gas_Agency_Management.xlsx) for full sprint planning, backlog, retrospective, and impediment tracking.

## Tech Stack / Tools

Pega Platform (App Studio), Case Management, Data Pages, Declare Expressions, Email Notifications, Work Queues

## Repository Contents

- `HLD_GAM_Pega_Challengers.pdf` — High-level design document
- `UAP_KLU_TCS02_Gas_Agency_Management.xlsx` — Sprint planning, backlog, and retrospectives
- Pega application export (rulesets/configuration)

---

*Academic project completed as part of Pega certification coursework.*
