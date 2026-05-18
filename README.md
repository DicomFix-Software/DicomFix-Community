# DicomFix-Community
Advanced DICOM metadata normalizer and compliance tool optimized for Radiotherapy Treatment Planning Systems (TPS) such as Varian Eclipse.

# DicomFix v3.8

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

### Custom Integrations
While DicomFix standard edition addresses common manufacturing non-compliances, oncology centers often deal with legacy or proprietary hardware. We offer custom developer support and tailored patch integration for specific scanner models and unique TPS error logs.

### Contact & Sponsorship
For custom enterprise deployments, technical inquiries, institutional sponsorship tiers, and custom developer support, please:
* Open a **technical or commercial support inquiry** via the **Issues** tab in this repository.
* Reach out to our team via our custom support and licensing channels.

---

## Legal & Terms of Use

### Copyright
Copyright (c) 2026. All rights reserved.

### License Terms
DicomFix Standard Edition is distributed as a pre-compiled, standalone executable free of charge for clinical, educational, and research use within medical physics and oncology departments.

* **Restrictions:** Modification, reverse-engineering, decompilation, disassembly, or commercial redistribution of the binary executable is strictly prohibited without explicit written authorization from the author.
* **Warranty:** This software is provided "as is" without warranty of any kind, express or implied. In no event shall the authors be liable for any claim, damages, or other liability arising from the use of the software.
