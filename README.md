# 🖨️ GuideOS Scanner Studio
Eine moderne, leistungsfähige Open-Source Desktop-Anwendung zur Ansteuerung von Flachbett- und Dokumentenscannern unter Linux (SANE-Schnittstelle) auf Basis von **PyQt6**, **OpenCV** und **Tesseract OCR**.

<div style="display:flex; gap:10px;">
  <img src="screenshots/screenshot_1.png" width="200">
  <img src="screenshots/screenshot_2.png" width="200">
</div>




![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)
![PyQt6](https://img.shields.io/badge/PyQt6-6.0+-41CD52?style=flat&logo=qt&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Linux-SCC300?style=flat&logo=linux&logoColor=white)
![License](https://img.shields.io/badge/License-GPLv3-blue.svg)
---

GuideOS Scanner Studio ist eine schlanke, grafische Python-Anwendung zur Ansteuerung von Flachbett-, Einzugs- (ADF) und Durchlicht-Scannern (Dias/Negative) über die Linux SANE-Schnittstelle. Es wurde speziell für eine zuverlässige Hardware-Interaktion (insbesondere mit netzwerk- und eSCL-basierten Ricoh-Multifunktionsgeräten) entwickelt.

Hauptfunktionen & Highlights
Integrierte Profilverwaltung: Vordefinierte und anpassbare Scanziele (z. B. PDF + OCR, ADF / Stapel, Fotos mit Autozuschnitt, Dias / Negative) inklusive Speicherung benutzerdefinierter Einstellungen.

Spezielle ADF-A4-Geometrie-Fixes: Erzwingt die vollständige DIN A4 Scanfläche bei jeder Einzugsseite, um Bildstauchungen und Treiber-Resets bei Geräten wie Ricoh MFPs zu verhindern.

Automatische Foto-Erkennung & Zuschnitt: Verwendet OpenCV-Konturensuche zur automatischen Erkennung, Entzerrung und Separierung mehrerer auf dem Flachbett liegender Fotos in einzelne Dokumentenseiten.

Integrierte Durchlicht- & Filmverarbeitung: Unterstützt Negativ-Invertierung und verarbeitet Durchlicht-Ausschnitte stabil per Software-Crop.

---   
### Sicherheits- & Usability-Features:

Automatische Sperre des Vorschau-Buttons bei aktivem ADF-Einzug zur Vermeidung von Hardware-Sperren.

Threading-basierter Systemstart mit Splash-Screen zur unterbrechungsfreien Hardware-Suche.

Unterstützung für native PNG-Button-Pixmaps (/usr/share/pixmaps/) für saubere Integration in Debian/Ubuntu-Pakete (.deb).

Integrierte Tesseract-OCR zur Erstellung durchsuchbarer PDFs.

---   
**Systemvoraussetzungen:** Linux (Debian/Ubuntu), Python 3, PyQt6, SANE, OpenCV, Pillow, Tesseract OCR, PyPDF
---     

## 🔧 Installation für Debian / Ubuntu / Linux Mint:

**Download des `.deb` Packages, von der **[Releases](https://https://github.com/GuideOS/guideos-scanner-studio/releases)** Section in diesem Repository**   \
**Öffne ein Terminal in deinem Download-Ordner und führe folgenden Befehl aus:**
```bash
sudo apt update
sudo apt install ./guideos-scanner-studio*.deb
```
