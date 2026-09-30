# VETCARE AI

VETCARE AI is a prototype for early livestock health screening, veterinary coordination, and disease-risk surveillance. It connects farmers, veterinarians, and authorities through a single digital workflow.

## Core Workflow

Farmer observes an animal  
↓  
Reports symptoms / observations  
↓  
VETCARE AI performs initial risk screening  
↓  
Case can be reviewed by a veterinarian  
↓  
Authorities can monitor alerts and surveillance

## Key Features

### Farmer Portal
- Animal registration and digital animal records
- Animal health passport and timeline
- Symptom-based health screening
- Voice-based symptom reporting
- Text and symptom-chip input
- Initial AI-assisted risk screening
- AI-assisted visual screening
- Vaccination records and reminders
- Document upload and management
- Animal QR code / passport access
- Milk yield logging
- Vet help and contact options
- Call veterinarian
- WhatsApp veterinarian communication
- Multilingual interface

### Offline-First Operation
- Works in both online and offline states
- Records can be saved locally when there is no internet connection
- Offline sync queue for pending records
- Sync when connectivity returns
- Sync conflict handling between farmer and veterinarian records

### Veterinarian Portal
- Veterinary dashboard
- Incoming case management
- Case acceptance and investigation
- Animal record and health history review
- Veterinary consultations
- Vaccination management
- Farmer contact
- Case resolution
- Surveillance and cluster monitoring

### Authority Portal
- District and village-level monitoring
- Alerts and surveillance
- Risk/cluster monitoring
- Investigation, acknowledgement and resolution of alerts
- Veterinary team coordination
- Campaign planning
- Target and reached animal tracking
- Analytics and surveillance views
- One Health / zoonotic-risk layer

### Communication
- Direct veterinarian calling
- WhatsApp-based veterinarian contact
- Farmer-to-veterinarian communication workflow

### Optional Sensor Monitoring
- BLE-based temperature and activity sensor concept
- Sensor information can be combined with farmer observations and animal records
- Sensor readings are simulated in this prototype for demonstration

## AI / Risk Screening

The prototype demonstrates:
- Symptom-based risk screening
- Animal-level risk indicators
- Cluster-risk indicators
- Risk timelines
- AI-assisted visual screening

The screening is intended as an early-warning and decision-support mechanism and is **not a veterinary diagnosis**.

## Prototype Status

This repository contains a demonstration prototype.

Some components, including sensor observations and demonstration screening logic, use simulated/demo data to show the proposed workflow.

Real-world deployment would require validated clinical models, real sensor hardware/integration, backend infrastructure, security controls, and appropriate integration with external/government systems.

## Goal

VETCARE AI aims to reduce the gap between:

**Early symptom → Farmer report → Risk screening → Veterinary review → Local surveillance and response**
