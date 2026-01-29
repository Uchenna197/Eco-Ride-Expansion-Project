
# Use Cases and User Stories – Eco-Ride Project

## 1. Purpose
This document captures the **key system interactions (use cases)** and **user-centered requirements (user stories)** for the Eco-Ride platform.

It bridges the gap between:
- Business requirements
- Functional requirements
- Solution design and testing

---

## 2. Actors

| Actor | Description |
|-----|------------|
| Rider | End user who books and uses Eco-Ride services |
| Driver | Operator providing rides using Eco-Ride vehicles |
| Admin | System administrator managing users, vehicles, and operations |
| Payment Gateway | External system that processes payments |
| GPS/Map Service | External system providing location and routing data |

---

## 3. High-Level Use Case Diagram (Textual)

**Rider**
- Register / Log in
- Search for available rides
- Book a ride
- Make payment
- Track ride
- Rate ride

**Driver**
- Log in
- Accept ride requests
- Start and complete rides
- View earnings

**Admin**
- Manage users
- Manage vehicles
- Monitor rides and payments
- Generate reports

---

## 4. Detailed Use Cases

### UC-01: User Registration

| Item | Description |
|----|------------|
| Use Case ID | UC-01 |
| Actor | Rider / Driver |
| Description | User creates a new account on the Eco-Ride platform |
| Precondition | User is not registered |
| Postcondition | User account is created successfully |
| Main Flow | 1. User opens app<br>2. Selects Register<br>3. Enters required details<br>4. System validates input<br>5. Account is created |
| Alternate Flow | If validation fails, system displays error message |

---

### UC-02: Book a Ride

| Item | Description |
|----|------------|
| Use Case ID | UC-02 |
| Actor | Rider |
| Description | Rider books an available Eco-Ride vehicle |
| Precondition | Rider is logged in |
| Postcondition | Ride request is confirmed |
| Main Flow | 1. Rider enters pickup and destination<br>2. System displays available vehicles<br>3. Rider selects vehicle<br>4. System confirms booking |
| Alternate Flow | If no vehicle is available, system displays notification |

---

### UC-03: Process Payment

| Item | Description |
|----|------------|
| Use Case ID | UC-03 |
| Actor | Rider |
| Supporting Actor | Payment Gateway |
| Description | Rider completes payment for a ride |
| Precondition | Ride is completed |
| Postcondition | Payment is successfully processed |
| Main Flow | 1. System calculates fare<br>2. Rider selects payment method<br>3. Payment is processed<br>4. Confirmation is displayed |
| Alternate Flow | Payment failure prompts retry option |

---

### UC-04: Driver Accepts Ride

| Item | Description |
|----|------------|
| Use Case ID | UC-04 |
| Actor | Driver |
| Description | Driver accepts a ride request |
| Precondition | Driver is logged in and available |
| Postcondition | Ride is assigned to driver |
| Main Flow | 1. Driver receives ride request<br>2. Accepts request<br>3. System assigns ride |

---

### UC-05: Admin Manages Vehicles

| Item | Description |
|----|------------|
| Use Case ID | UC-05 |
| Actor | Admin |
| Description | Admin adds, updates, or deactivates vehicles |
| Precondition | Admin is authenticated |
| Postcondition | Vehicle data is updated |
| Main Flow | 1. Admin logs in<br>2. Views vehicle list<br>3. Adds/updates vehicle details |

---

## 5. User Stories

### Rider User Stories
- As a **rider**, I want to register easily so that I can access Eco-Ride services.
- As a **rider**, I want to see available vehicles near me so that I can book quickly.
- As a **rider**, I want to track my ride in real time so that I know when I will arrive.
- As a **rider**, I want to pay securely so that my financial information is protected.
- As a **rider**, I want to rate my ride so that service quality improves.

---

### Driver User Stories
- As a **driver**, I want to receive ride requests so that I can accept them promptly.
- As a **driver**, I want to view my earnings so that I can track my income.
- As a **driver**, I want to navigate using GPS so that I reach destinations efficiently.

---

### Admin User Stories
- As an **admin**, I want to manage users so that only valid users access the system.
- As an **admin**, I want to monitor rides so that I can ensure smooth operations.
- As an **admin**, I want to generate reports so that I can analyze business performance.

---

## 6. Acceptance Criteria (Sample)

**User Story:** Book a Ride  
- Given the rider is logged in  
- When a valid pickup and destination are entered  
- Then available vehicles are displayed  
- And the rider can confirm a booking successfully

---

## 7. Traceability
Each use case and user story is traceable to:
- Business Requirements Document (BRD)
- Functional Requirements
- Non-Functional Requirements
- UAT test cases

---

## 8. Notes
- Detailed screen flows and wireframes are documented in the Solution Design folder.
- Test cases derived from these user stories are documented in the Testing folder.

---
