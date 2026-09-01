<!--
  Version: 1.0.0
  Date: 2026-09-01
-->
# KDSF 2.1 Controlled Vocabularies & Value-Pairs for DSpace / DSpace-CRIS

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22226273.svg)](https://doi.org/10.5281/zenodo.22226273)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![KDSF Version](https://img.shields.io/badge/KDSF-v2.1-blue.svg)](https://kerndatensatz-forschung.de/)
[![DSpace Compatibility](https://img.shields.io/badge/DSpace--CRIS-7.x%20%7C%208.x%20%7C%209.x-orange.svg)](https://github.com/4Science/DSpace)

[English](#english) | [Deutsch](#deutsch)

---

## English

### Overview
This repository provides a complete, standardized, and validated implementation of the **Kerndatensatz Forschung (KDSF) Version 2.1** controlled vocabularies and `Value-Pairs` configurations for **DSpace** and **DSpace-CRIS** (versions 7.x, 8.x, and 9.x).

It encompasses all KDSF classification registries (`Klassif-L-1` through `Klassif-L-70`), covering the full metadata spectrum across:
* **B-1:** Academic Staff & Employment (`kdsf.*`)
* **B-2 / B-3:** Doctoral Candidates & Dissertations
* **B-4:** Habilitations
* **B-5:** Third-Party Funded Research Projects
* **B-6 / B-7 / B-8:** Scientific Publications & Open Access Typologies
* **B-9 – B-12:** Patents, Intellectual Property Rights & Exploitation
* **B-13:** Research Infrastructures & Equipment
* **B-14:** Organizational Units & Destatis Subject Classifications
* **B-15:** External Organizations & Funding Bodies
* **B-16 / B-17:** Spin-offs, Knowledge Transfer & Academic Awards

### Repository Structure
* `controlled-vocabularies/`: 88 well-formed, UTF-8 encoded XML controlled vocabulary files designed for `[dspace]/config/controlled-vocabularies/`.
* `submission-forms/`: Consolidated `submission-forms-kdsf-valuepairs.xml` containing ready-to-use `<value-pairs>` blocks for `[dspace]/config/submission-forms.xml`.

### Installation & Deployment

1. **Deploy Controlled Vocabularies:**
   Copy the contents of `controlled-vocabularies/` into your DSpace configuration folder:
   ```bash
   cp controlled-vocabularies/*.xml [dspace]/config/controlled-vocabularies/
