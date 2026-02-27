# Swift Pay — QA Review: "Scan to Pay" (QR) Feature

## Overview

This repository contains the completed **QA Review Template** for the **"Scan to Pay"** QR code payment feature of **Swift Pay**, a fictional Ghanaian fintech mobile application. The review was completed as part of a Module Lab capstone on Software Testing and Quality Assurance.

## Feature Under Review

| Detail | Value |
|--------|-------|
| **Document** | FS-P2M-v1.0: "Scan to Pay" (QR) |
| **Feature** | Peer-to-Merchant (P2M) QR code payments |
| **Scope** | Scan merchant QR → Enter amount → Confirm with PIN → Payment processed |

## Deliverables

| File | Description |
|------|-------------|
| `Quality Review for Swift Pay.pdf` | Completed QA Review Template with test cases, bug report, and process improvement suggestion |

## What's Inside the Review

### Part 1 — Test Cases


- **TC-01 (Happy Path):** End-to-end successful payment flow covering acceptance criteria AC-01 through AC-07.
- **TC-02 (Negative / Edge Case):** Repeated incorrect PIN entry scenario, highlighting a missing retry-limit specification — a security concern for fintech applications.

### Part 2 — Bug Report

- **BUG-01:** The UI mockup's amount input field is always editable, contradicting AC-09 which requires the field to be read-only when the QR code contains an embedded amount. Classified as **High Severity / High Priority**.

### Part 3 — Process Improvement

A **Shift Left** recommendation from a data specialist perspective: implement a specification-to-mockup traceability matrix during the design phase to ensure every acceptance criterion maps to a corresponding UI state before development begins.


## Author

*[Your Name]* — Data Specialist

## License

This project is for educational purposes as part of a Software Testing module lab.