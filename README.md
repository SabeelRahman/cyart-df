# Week-3: Digital Forensics & Malware Analysis Capstone

**Examiner:** Syed Sabeelur Rahman  
**Date:** 2026-03-25  
**Case:** WEEK3-TRAINING

## Overview
This repository contains my deliverables for the Week-3 Forensics Capstone. I completed a full forensic investigation workflow, including evidence collection, disk analysis, network traffic analysis, registry examination, and malware analysis (static + dynamic).

## What I Did
1. **Evidence Collection:** Created a simulated USB image and forensically imaged it using ewfacquire. Verified integrity with SHA-256 hashing.
2. **Disk Analysis:** Used Autopsy 2.24 to recover files and search for keywords like CONFIDENTIAL and password.
3. **Network Analysis:** Captured traffic with Wireshark and analyzed baseline behavior.
4. **Registry Analysis:** Used RegRipper 3.0 to extract artifacts like RecentDocs and UserAssist.
5. **Malware Analysis:** Performed static string extraction and dynamic sandbox analysis (Hybrid Analysis) to identify IOCs and MITRE ATT&CK techniques.

## Repository Structure
Week-3/
├── 02-Evidence-Collection/   # Forensic images and hash verification
├── 03-Autopsy-Analysis/      # Autopsy case files
├── 04-Network-Analysis/      # Wireshark captures
├── 05-Registry-Analysis/     # RegRipper output
├── 06-Static-Malware/        # Static analysis reports
├── 07-Dynamic-Malware/       # Sandbox analysis reports
├── 08-Capstone-Deliverables/ # Final reports and timeline
└── screenshots/              # Evidence screenshots

## Tools Used
- Imaging: ewfacquire, dd
- Analysis: Autopsy 2.24, RegRipper 3.0, Wireshark
- Malware: strings, Hybrid Analysis, ANY.RUN

## Verification
All evidence files maintain cryptographic integrity. Hash values are documented in chain_of_custody.txt and hash_verification_report.txt.

## Notes
- This is a training exercise using simulated evidence.
- No real malware was executed on my local system.
- Dynamic analysis was performed in isolated cloud sandboxes.
