# DicomFix v3.10.0 Pro

DicomFix is an advanced, high-performance medical imaging utility designed to analyze, normalize, and cure DICOM datasets for strict compatibility and seamless integration into demanding Radiotherapy Treatment Planning Systems (TPS), such as Varian Eclipse.

Clinical environments often encounter critical import failures due to manufacturer-specific non-compliances, corrupt metadata, or compressed transfer syntaxes. DicomFix acts as a robust gateway, ensuring that all datasets imported into your clinical planning system are standard-compliant and structurally perfect.

---

## Core Capabilities

DicomFix provides an advanced, automated pipeline to diagnose and cure compliance irregularities in medical datasets without altering standard, high-fidelity geometry or vital clinical parameters:

* **Syntax & Physical Decompression:** Transcodes compressed pixel data (JPEG Lossless/RLE) into native uncompressed Implicit VR Little Endian, solving transfer syntax mismatches and ensuring smooth rendering on native radiotherapy consoles.
* **Identity Compliance Pipeline:** Validates patient credentials (such as Patient Name and Patient ID) against strict Value Representation (VR) length constraints. Features an interactive, supervised UI dialog for batch identity management when standard violations are detected, ensuring clinical safety and traceability.
* **Mandatory Type 1 Attributes Fix:** Automatically detects and injects missing or empty mandatory MR acquisition and scanning attributes required by strict clinical validation engines to prevent sudden series rejection in the TPS.
* **Geometric Series Segregation:** Automatically isolates mixed dataset components (such as localizer/scout sequences) into independent logical series. This prevents multi-dimensional volume reconstruction failures, 3D planning errors, and spatial orientation conflicts in the TPS.
* **Private Metadata Purge:** Eradicates malformed, non-standard private manufacturer tags that violate VR constraints, bypass standard compliance, or corrupt database indexing.
* **Folder Structure Replication:** Processes massive cohorts of patient data asynchronously while maintaining the original, complex source folder hierarchy perfectly in the output directory.

---

## User Interface Overview

DicomFix is equipped with a premium, high-performance workstation interface designed specifically for clinical medical physics and dosimetry environments:

* **Explorer Panel:** An interactive tree explorer that scans and maps entire patient databases recursively, allowing granular workspace, folder, or file-level selection.
* **Diagnostic Console:** A high-performance table that maps detected data irregularities to precise, descriptive suggested technical actions, ensuring full operator awareness before applying fixes.
* **Interactive Tooltips:** Instant availability of full technical diagnostic details and problem logs via interactive hover tooltips on diagnostic cells.
* **Integrated Radiotherapy Viewer:** A clinical-grade viewport featuring real-time interactive window/level (W/L) adjustments to visually inspect images.

---

## Technical Stack & Distribution

* **Environment:** Python 3.11+
* **Dependencies:** Built upon standard libraries including `pydicom`, `PySide6`, `numpy`, and `pylibjpeg`.
* **Security & Protection:** Distributed executable binaries are fortified via automated PyArmor obfuscation within our build pipelines to protect advanced intellectual property and proprietary normalization methods.
* **Installation:** No local Python installation required. Download the standalone executable directly from the **Releases** section of this repository.

---

## Commercial & Support

### Premium & Pro Features
DicomFix v3.10.0 Pro includes advanced, high-performance integration and diagnostic tools for medical physics workflows:
* **Automated Audit PDF Reports**: Programmatically compiles clinical-grade PDF compliance certificates documenting all tag normalizations, private tag purges, and MR coordinate corrections. Features an explicit *Mathematical & Geometric Integrity Check* validating that the pixel matrix, voxel spacing, and patient coordinates (`Image Position` / `Image Orientation`) were preserved 100% untouched for absolute dosimetric and geometric safety. Review diagnostics dynamically through the in-app interactive HTML facsimile and save reports to your clinical records.
* **Side-by-Side DICOM Header Compare**: Instantly compares source and fixed metadata headers side-by-side to review exact compliance transformations, normalization details, and value changes before exporting.
* **Advanced Research Anonymizer**: Clinical research de-identification and de-identification tool designed to scrub patient identifiers, regenerate critical UIDs, and prepare datasets for secure multi-center research or clinical trials under strict privacy regulations.

These advanced capabilities are premium tools that can be activated upon custom request to the developer. We operate on a collaborative, peer-to-peer model, providing direct, personalized technical assistance to help you with workstation setup, scanner integration, and custom clinical workflow optimization.

### Professional Collaboration & Communication Channels
We provide direct technical support and customized onboarding to help you integrate DicomFix into your clinical environment (e.g., custom legacy hardware integration or specific TPS error logs). You can reach out directly via our three official, personalized communication channels:

* **Official GitHub Community Issues Workspace**: https://github.com/DicomFix-Software/DicomFix-Community/issues
* **LinkedIn Direct Messaging Pipeline**: https://www.linkedin.com/in/miguel-angel-yanez-sanchez/
* **Direct Secure Professional Email**: miguelyanez18@gmail.com

---

## ⚖️ Legal Declarations & Disclaimer

### Copyright
Copyright © 2026 Miguel Ángel Yánez Sánchez. All rights reserved. 
DicomFix® and DicomFix Pro® are proprietary software utilities. Unauthorized copying, distribution, modification, or reverse engineering of the binary executables or source layout configurations via any medium is strictly prohibited without the express written permission of the author.

### Medical Disclaimer & Liability
DicomFix is an advanced data-normalization utility intended exclusively for metadata compliance analysis, clinical research de-identification, and technical data auditing. It is NOT cleared as an active Medical Device by the FDA, CE, or any regulatory body. 

The software does not alter high-fidelity clinical coordinates, voxel spatial dimension vectors, or pixel matrices. However, the final certified Medical Physicist or Radiation Oncologist retains absolute, non-delegable responsibility for verifying and validating the geometric, spatial, and dosimetric integrity of any dataset before importing it into a Treatment Planning System (TPS) or utilizing it for active human clinical treatment. The author assumes zero liability for clinical planning errors, database synchronization defects, or treatment deviations arising from the use of this software.