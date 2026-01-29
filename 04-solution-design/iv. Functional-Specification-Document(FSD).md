
# Functional Specification Document (FSD) – Eco-Ride

## 1. Purpose
This document defines the **functional behavior** of the Eco-Ride system and serves as input for development and testing.

---

## 2. System Components
- Mobile Application (Rider & Driver)
- Admin Dashboard
- Payment Integration
- GPS & Mapping Service

---

## 3. Functional Specifications

### FS-01 User Registration
- Users shall register using email or phone number
- System shall validate user credentials
- System shall create a user profile

---

### FS-02 Ride Booking
- Rider shall enter pickup and destination
- System shall display available vehicles
- Rider shall confirm booking
- System shall notify assigned driver

---

### FS-03 Ride Tracking
- System shall display driver location in real time
- Rider shall view estimated arrival time

---

### FS-04 Payment Processing
- System shall calculate fare automatically
- Rider shall select payment method
- System shall confirm payment status

---

### FS-05 Ratings & Feedback
- Rider shall rate completed rides
- System shall store ratings for reporting

---

## 4. Business Rules
- Only verified drivers can accept rides
- Payment must be successful before ride completion
- Ratings are mandatory after ride completion

---

## 5. Error Handling
- System shall display user-friendly error messages
- Failed payments shall allow retry

---

## 6. Assumptions & Constraints
- Internet connectivity is required
- Third-party APIs are available and reliable

---
