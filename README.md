# Medora
# 🏥 Medora

### AI-Powered Digital Health Records Platform with Secure QR Sharing

> **One Medical History. Anywhere. Anytime.**

Medora is a **B2B2C healthcare platform** that enables hospitals, clinics, doctors, and patients to securely manage, access, and share medical records through AI-powered summarization and time-limited QR-based access.

Instead of carrying bulky physical reports or searching through WhatsApp chats during consultations, patients can instantly share their complete medical history with any doctor using a secure QR code. Hospitals upload records directly into the platform, AI automatically generates structured medical summaries, and doctors receive organized information within seconds.

---

# ✨ Key Features

## 👤 Patient App

* Secure Authentication
* Digital Medical Record Storage
* Folder-wise Organization
* AI Generated Medical Summaries
* Background Summary Refresh
* Family Record Management
* Time-limited QR Generation
* Complete Medical Timeline

---

## 🏥 Hospital Dashboard

* Patient Registration
* Medical Report Upload
* Patient Record Management
* Doctor Management
* Secure File Storage
* Role-based Access Control
* Audit Logging

---

## 👨‍⚕️ Doctor Portal

* QR Verification
* Instant Patient History
* AI Generated Clinical Summary
* Read-only Access
* No Patient App Installation Required

---

# 🚀 Complete Workflow

```
Hospital uploads reports
          │
          ▼
Reports stored securely
          │
          ▼
OCR extracts report contents
          │
          ▼
AI generates structured summaries
          │
          ▼
Summaries stored in database
          │
          ▼
Patient receives updated records
          │
          ▼
Patient generates secure QR
          │
          ▼
Doctor scans QR
          │
          ▼
QR verification
          │
          ▼
Pre-generated summaries served instantly
```

---

# 🧠 AI Pipeline

Instead of generating summaries every time a doctor scans a QR, Medora performs AI processing **proactively**.

Whenever:

* New reports are uploaded
* Existing reports are modified
* Background scheduler detects changes

the system automatically:

```
Medical Reports
        │
        ▼
OCR Extraction
        │
        ▼
Sensitive Data Masking
        │
        ▼
Gemini AI
        │
        ▼
Multiple Summary Types
        │
        ▼
Summary Database
```

Different summary formats are generated in advance, such as:

* Complete Medical History
* Doctor Consultation Summary
* Emergency Summary
* Medication Summary
* Allergies
* Chronic Diseases
* Recent Reports
* Laboratory Findings

These summaries are cached and refreshed periodically, enabling doctors to receive results instantly without waiting for AI inference.

---

# 🔄 Data Flow

```
                Hospital Dashboard
                        │
                        ▼
              Medical Report Upload
                        │
                        ▼
              Secure Object Storage
                        │
                        ▼
               OCR Text Extraction
                        │
                        ▼
               Background AI Engine
                        │
                        ▼
          Structured Medical Summaries
                        │
         ┌──────────────┴──────────────┐
         ▼                             ▼
 Patient Database              Summary Database
         │                             │
         └──────────────┬──────────────┘
                        ▼
                QR Token Generation
                        │
                        ▼
                 Doctor QR Scan
                        │
                        ▼
                QR Authentication
                        │
                        ▼
            Fetch Pre-generated Summary
                        │
                        ▼
             Doctor Read-only Interface
```

---

# 🔐 Security Architecture

Medora follows a **Zero-Trust Security Model**.

### Authentication

* JWT Authentication
* Refresh Tokens
* Role-Based Access Control (RBAC)

### Authorization

* Patient
* Doctor
* Hospital Admin
* Super Admin

### Data Protection

* Encrypted Storage
* Signed File URLs
* Short-lived QR Tokens
* Time-limited Access
* Audit Logging
* Secure API Gateway

### AI Privacy

Before sending data for AI summarization:

* Personal identifiers are masked
* Sensitive information is anonymized where applicable
* Only required clinical content is processed

---

# 📱 QR Sharing Flow

```
Patient
   │
Generate QR
   │
   ▼
Secure Token Created
   │
   ▼
Doctor Scans QR
   │
   ▼
Backend Verifies Token
   │
   ▼
Access Permissions Checked
   │
   ▼
Retrieve Cached Summary
   │
   ▼
Doctor View Opens
```

No account creation is required for doctors to view shared records.

---

# 🏗 System Architecture

```
Flutter Mobile App
        │
        ▼
 REST API Gateway
        │
        ▼
 Node.js Backend
        │
 ┌──────┴────────┐
 ▼               ▼
Database     Object Storage
 │               │
 ▼               ▼
Summary DB   Medical Reports
      │
      ▼
 Background AI Workers
      │
      ▼
 Gemini AI
```

---

# ⚙️ Technology Stack

| Layer          | Technology                     |
| -------------- | ------------------------------ |
| Frontend       | React, React-Native, Typescript|
| Backend        | Node.js + Express              |
| Database       | Supabase                       |
| Authentication | JWT                            |
| File Storage   | Object Storage (S3 Compatible) |
| OCR            | Vertex AI                      |
| AI             | Gemini API                     |
| QR             | Secure Token-based QR          |
| Scheduler      | Background Workers / Cron Jobs |

---

# 🎯 Mission

Our mission is to eliminate fragmented healthcare records by providing a secure, AI-powered infrastructure that enables patients, hospitals, and doctors to exchange medical information instantly while preserving privacy, reducing duplicate tests, and improving clinical decision-making.

---

# 🌟 Vision

To become the digital health record infrastructure powering seamless medical data exchange across hospitals, clinics, and patients.

---

# 📌 Current Status

🚧 Active Development

Current focus includes:

* Secure Medical Record Management
* AI Summarization Pipeline
* Background Summary Generation
* QR-based Doctor Access
* Zero-Trust Security Architecture
* Production-ready Infrastructure

---

## 📄 License

This project is proprietary software.

All rights reserved © Medora.

Unauthorized copying, distribution, modification, or commercial use of this software is prohibited without explicit permission from the authors.


