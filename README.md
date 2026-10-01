# vetcare-ai
AI-assisted livestock health screening and surveillance prototype connecting farmers, veterinarians, and authorities.


🛡️ VETCARE AI
VETCARE AI is a prototype for early livestock health screening, veterinary coordination, and disease-risk surveillance.
It connects farmers, veterinarians, and authorities through a unified digital workflow for animal health reporting, initial risk screening, veterinary case management, alerts, surveillance, and response coordination.

Prototype: This project demonstrates the proposed workflow and user experience. It is not a production veterinary diagnostic system.

🚀 Core Workflow

Animal shows early signs
        ↓
Farmer reports symptoms / observations
        ↓
VETCARE AI performs initial risk screening
        ↓
Animal health history and other available signals are reviewed
        ↓
Veterinarian reviews the case
        ↓
Authority monitors alerts, clusters and surveillance
        ↓
Response / campaign / field action

👨‍🌾 Farmer Portal

Animal registration and digital animal records

Animal health passport and timeline

Symptom-based health screening

Text and voice-based symptom reporting

Tap-and-speak interaction

Multilingual interface

Initial AI-assisted risk screening

AI-assisted visual screening

Animal QR code / passport access

Vaccination records and reminders

Document upload and management

Milk yield logging and trends

Veterinarian help

Direct veterinarian calling

WhatsApp veterinarian communication

Nearest veterinarian information

Vaccine availability/need views

Sale/health status workflow

Antimicrobial and milk-safety information

📶 Offline-First Operation

Online/offline state indication

Save records when offline

Local data persistence

Offline synchronization queue

Pending-sync record tracking

Sync when connectivity is restored

Sync conflict handling

Farmer-record vs veterinarian-record resolution

Merge / keep-farmer / keep-vet options

🩺 Veterinarian Portal

Veterinary dashboard

Incoming cases and filtering

Case acceptance and investigation

Animal record and health-history review

Farmer contact

Veterinary consultations

Findings and action planning

Prescription information

Vaccination management

Case resolution

Surveillance and cluster monitoring

🏛️ Authority Portal

District and village monitoring

Farm and animal monitoring

Alerts and suspected clusters

Surveillance map

Risk analytics and timelines

Seven-day risk forecasting concept

Disease-risk network visualization

Veterinary team coordination

Alert investigation, acknowledgement and resolution

Team deployment

Village notification

Campaign planning

Ring-vaccination workflow

Targeted/reached animal tracking

🤖 AI-Assisted Health Screening

The prototype demonstrates:

Symptom-based risk screening

Animal-level risk indicators

Risk scores and reasons for flagged animals

Risk timelines

Cluster-risk indicators

AI-assisted visual screening

Observable-abnormality screening

Recommended next steps

Herd/village risk signals

Disease-risk alerts

Important: Screening is intended as early warning and decision support. It does not confirm disease or replace veterinary diagnosis.

🎙️ Voice & Multilingual Support

Voice-based symptom input

Speech-to-text workflow

Read-aloud support

Multiple Indian-language interface options

Language selection

Bhashini voice/API integration concept

📞 Communication

Direct veterinarian calling

WhatsApp veterinarian contact

Farmer-to-veterinarian workflow

SMS communication concept

IVR communication concept

Contact information shown in the prototype is demonstration data.

📡 Optional Sensor Monitoring

VETCARE AI is designed to be sensor-optional.

Sensor concept: BLE Temperature + Activity

Animal
   ↓
Optional BLE sensor
   ↓
Temperature / activity observations
   ↓
VETCARE AI
   ↓
Combined with farmer observations,
animal history and other available data
   ↓
Initial risk screening

Animals without a sensor can still use the core screening workflow using farmer inputs and available animal information.

Prototype note: Sensor observations are simulated/demo data. Physical sensor hardware is not required to demonstrate the prototype.

🥛 Milk Yield & Dairy Information

Milk yield logging

Litres and fat percentage

Milk-yield trends

Milk society information

Milk-safety workflow

Withdrawal-period information

Residue-risk information

Sale/health status concepts

Milk information can act as an additional animal-health signal alongside symptoms and other observations.

💉 Vaccination & Animal Health Records

Vaccination records

Upcoming and overdue vaccinations

Next-due information

Vaccination certificates

Health timeline

Digital health passport

Animal QR access

Birth records

Prescriptions

Lab reports

Deworming records

Breeding records

Ownership information

Sale passport

Death certificates

💊 Antimicrobial & Milk Safety

Prescription information

Drug information

Antimicrobial categories

Withdrawal periods

Milk safety status

Residue-risk indicators

These features are workflow/information support and not independent medical prescribing.

🌍 One Health Layer

The prototype includes a One Health / zoonotic-risk layer for:

Animal health

Herd risk

Village risk

Zoonotic-risk signals

Public-health notification concepts

These signals flag potential concerns and do not confirm a zoonotic disease.

🗺️ Maps, Weather & Field Context

Surveillance map

Village locations

Veterinarian locations

Animal markets / haats

Weather information

Risk mapping

Disease-risk network

Village-level risk views

The map interface uses Leaflet.

🔗 Data & Integration Architecture

                         VETCARE AI
                              |
          +-------------------+-------------------+
          |                   |                   |
        Farmer               Vet              Authority
          |                   |                   |
          +-------------------+-------------------+
                              |
                     VETCARE AI ENGINE
                              |
             +----------------+----------------+
             |                |                |
        Risk Engine     Cluster Engine       Alerts
             |
             ↓
       Integration / API Layer
             |
     +-------+---------+---------+---------+
     |                 |         |         |
Bharat Pashudhan   Bhashini   SMS/IVR    Weather
   / NADRS           Voice       APIs      / IMD

The prototype includes integration concepts for:

Pashu Aadhaar / NADRS

Bhashini voice services

SMS / IVR

Weather information

External API integration

Government integration status

The government/NADRS endpoints represented in the prototype are mock/demo endpoints. Real integration would require appropriate government onboarding, authentication, permissions, infrastructure, and production APIs.

🆔 Pashu Aadhaar / NADRS Integration Concept

Animal synchronization status

Pending synchronization status

Bulk synchronization workflow

Animal API concept

Vaccination API concept

Individual animal lookup concept

Village/herd lookup concept

These are demonstrated through mock integration endpoints in the prototype.

🔌 API Architecture

Farmer / Vet / Authority
          ↓
    VETCARE AI Engine
          ↓
   Risk / Cluster / Alerts
          ↓
    Integration Layer
          ↓
 External Government / Service APIs

The architecture allows future replacement of demonstration data and mock endpoints with validated production integrations.

🔐 Authentication & Roles

The prototype demonstrates role-based workflows for:

Farmer

Veterinarian

Authority

It includes:

Mobile/OTP login concept

Staff ID/password login concept

Demo login

Role selection

State selection

Language selection

Logout

The credentials and contact information included in the prototype are demonstration data.

🌐 Supported Regional Languages

The prototype includes multilingual interface support for:

English

Hindi

Kannada

Malayalam

Marathi

Tamil

Telugu

Bengali

Gujarati

Punjabi

Voice language options are also represented through the voice-service integration concept.

🧪 Prototype / Demo Data

This repository is a demonstration prototype.

Some data is intentionally simulated, including:

Animal records

Farmer records

Veterinarian records

Alerts

Risk observations

Sensor observations

Example contacts

Demonstration login credentials

Mock government/NADRS integration endpoints

This allows the complete workflow to be demonstrated without requiring a production backend.

⚠️ Prototype Limitations

Real-world deployment would require:

Clinically validated disease-risk models

Real veterinary datasets

Real sensor hardware and device integration

Secure backend infrastructure

Production authentication

Data privacy and security controls

Government API onboarding

Validated external integrations

Field testing

Veterinary and regulatory validation

Production monitoring and maintenance

🛠️ Technology / Implementation

The prototype is implemented as a web-based HTML application with client-side JavaScript and CSS.

It uses or demonstrates:

HTML

CSS

JavaScript

Browser-based local data handling

Leaflet map interface

Voice/API integration concepts

Responsive mobile-oriented UI

External services shown in the prototype are used as integration concepts or demonstration dependencies where applicable.

▶️ Running the Prototype

Option 1 — Open locally

Download/clone the repository and open:

index.html

in a modern web browser.

Option 2 — GitHub Pages

The prototype can be hosted using GitHub Pages as a static web application.

Recommended repository structure:

vetcare-ai/
├── index.html
└── README.md

🎯 Goal

VETCARE AI aims to reduce the gap between the first observation of an animal-health problem and coordinated veterinary response.

Early Symptom
      ↓
Farmer Report
      ↓
Risk Screening
      ↓
Veterinary Review
      ↓
Local Response
      ↓
Authority Surveillance

VETCARE AI

Detect the silent signs. Act before disease spreads.
