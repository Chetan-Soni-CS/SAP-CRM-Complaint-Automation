# SAP CRM Complaint Automation (Python)

## Overview
This project demonstrates a Python-based automation solution for downloading complaint data and attachments from SAP CRM.
It is designed to replace repetitive manual workflows with a scalable and auditable automation process.

> ⚠️ Note: This is a sanitized version of an enterprise workflow.  
> No real credentials, URLs, or confidential data are included.

---

## Problem Statement
In large-scale service organizations, complaint attachments in SAP CRM are often downloaded manually.
This process is:
- Time-consuming
- Error-prone
- Not scalable for high complaint volumes
- Difficult to audit

---

## Solution Approach
Built an end-to-end Python automation that:
- Logs into SAP CRM using browser automation
- Searches complaints using Transaction / Complaint IDs
- Navigates complaint records reliably
- Downloads all available attachments
- Organizes files complaint-wise in structured folders
- Handles SAP-specific behaviors (e.g., images opening in new tabs)

---

## Key Features
- Automated SAP CRM navigation using Selenium
- Complaint-wise attachment download
- Dynamic folder creation per complaint ID
- File-type handling for PDFs, images, ZIPs, videos
- Retry and wait logic for slow-loading SAP elements
- Scalable design for large complaint volumes

---

## Technology Stack
- Python
- Selenium
- Requests
- Pandas (Excel input handling)

---

## Input & Output
**Input**
- Excel file containing Complaint / Transaction IDs

**Output**
- Structured folders with downloaded attachments:Output/
├── Complaint_12345/
│ ├── invoice.pdf
│ ├── image1.jpg
│ └── video.mp4


---

## Business Impact
- ~90% reduction in manual effort
- Faster complaint analysis and DOA investigations
- Improved audit readiness and traceability
- Consistent and repeatable execution

---

## Use Cases
- Market Quality teams
- Service Operations
- Complaint Analytics
- DOA and Field Failure investigations

---

## Disclaimer
This project is for educational and demonstration purposes only.
All logic is generalized and does not expose proprietary systems or data.

