# KDSF 2.1 Controlled Vocabularies & Value-Pairs for DSpace / DSpace-CRIS

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![KDSF Version](https://img.shields.io/badge/KDSF-v2.1-blue.svg)](https://kerndatensatz-forschung.de/)
[![DSpace Compatibility](https://img.shields.io/badge/DSpace--CRIS-7.x%20%7C%208.x-orange.svg)](https://github.com/4Science/DSpace)

[English](#english) | [Deutsch](#deutsch)

---

## English

### Overview
This repository provides a complete, standardized, and validated implementation of the **Kerndatensatz Forschung (KDSF) Version 2.1** controlled vocabularies and `Value-Pairs` configurations for **DSpace** and **DSpace-CRIS** (7.x and 8.x).

It encompasses all KDSF classification registries (`Klassif-L-1` through `Klassif-L-70`), covering the full metadata spectrum across:
* **B-1:** Academic Staff & Employment (`kdsf.*`)
* **B-2 / B-3:** Doctoral Candidates & Dissertations
* **B-4:** Habilitations
* **B-5:** Third-Party Funded Research Projects
* **B-6 / B-7 / B-8:** Scientific Publications & Open Access Typologies
* **B-9 - B-12:** Patents, Intellectual Property Rights & Exploitation
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
   ```

2. **Integrate Value-Pairs:**
   Merge the `<value-pairs>` elements from `submission-forms/submission-forms-kdsf-valuepairs.xml` into your local `[dspace]/config/submission-forms.xml` inside the `<form-value-pairs>` root element.

---

## Deutsch

### Ueberblick
Dieses Repository stellt eine vollstaendige, standardisierte und validierte Implementierung der kontrollierten Vokabulare und `Value-Pairs`-Konfigurationen des **Kerndatensatz Forschung (KDSF) Version 2.1** fuer **DSpace** und **DSpace-CRIS** (7.x und 8.x) bereit.

Es umfasst alle KDSF-Klassifikationslisten (`Klassif-L-1` bis `Klassif-L-70`) und bildet das vollstaendige Metadatenspektrum der KDSF-Module ab:
* **B-1:** Beschaeftigte und Beschaeftigungsverhaeltnisse (`kdsf.*`)
* **B-2 / B-3:** Promovierende und Promotionen
* **B-4:** Habilitationen
* **B-5:** Drittmittelprojekte und Foerderprogramme
* **B-6 / B-7 / B-8:** Publikationen und Open-Access-Typologien
* **B-9 - B-12:** Patente, Schutzrechte und Verwertung
* **B-13:** Forschungsinfrastrukturen und Geraete
* **B-14:** Organisationseinheiten und Destatis-Faechersystematik
* **B-15:** Drittorganisationen und Mittelgeber
* **B-16 / B-17:** Ausgruendungen, Transferaktivitaeten und Preise

### Repository-Struktur
* `controlled-vocabularies/`: 88 valide, UTF-8-kodierte XML-Dateien fuer das Verzeichnis `[dspace]/config/controlled-vocabularies/`.
* `submission-forms/`: Aggregierte Datei `submission-forms-kdsf-valuepairs.xml` mit einsatzbereiten `<value-pairs>`-Definitionen fuer `[dspace]/config/submission-forms.xml`.

### Installation und Einbindung

1. **Kontrollierte Vokabulare bereitstellen:**
   Kopieren Sie die XML-Dateien in das DSpace-Konfigurationsverzeichnis:
   ```bash
   cp controlled-vocabularies/*.xml [dspace]/config/controlled-vocabularies/
   ```

2. **Value-Pairs einbinden:**
   Fuegen Sie die `<value-pairs>`-Elemente aus `submission-forms/submission-forms-kdsf-valuepairs.xml` in den Bereich `<form-value-pairs>` Ihrer Datei `[dspace]/config/submission-forms.xml` ein.

---

## Author & Citation / Autor & Zitation

**Oleh Riabtsev**  
Universitaet Vechta, Germany  

## License / Lizenz
This work is licensed under a [Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE).
