# 📸 GuideOS Scanner Studio
Eine moderne, PyQt6-basierte Desktop-Anwendung für Linux zur komfortablen Steuerung von Dokumenten- und Fotoscannern über SANE.

<div style="display:flex; gap:10px;">
  <img src="screenshots/screenshot_1.png" width="200">
  <img src="screenshots/screenshot_2.png" width="200">
</div>

Das Tool bietet eine visuelle Vorschau mit manueller Bereichsauswahl, ein flexibles Profilsystem sowie eine automatische Objekterkennung und Entzerrung für Fotos und Dokumente (inkl. OCR-Unterstützung).

✨ Features
Anpassbare Scan-Profile: Wechsel schnell zwischen vorgefertigten oder eigenen Einstellungen für Dokumente, Einzelfotos oder Stapelscans.
Dynamische Objekterkennung (Auto-Crop & Deskew): Automatische Erkennung, Entzerrung und separates Speichern mehrerer auf dem Scanner platzierter Fotos.
Durchsuchbare PDFs (OCR): Erstellt auf Wunsch direkt durchsuchbare PDF-Dateien mittels Tesseract OCR.
Interaktive Vorschau: Rahmen per Maus aufziehen, um gezielt nur bestimmte Bereiche der Scanfläche zu erfassen.
Bildoptimierung: Direktes Anpassen von Helligkeit und Kontrast nach dem Scanvorgang.
Persistente Einstellungen: Benutzerdefinierte Profile werden automatisch im Home-Verzeichnis unter ~/.config/scanner_app/profiles.json gespeichert.
🛠️ Voraussetzungen
Das Programm basiert auf Python 3, PyQt6, OpenCV und dem SANE-Back-End.

System-Pakete installieren (Debian / Ubuntu / Linux Mint)
```bash
sudo apt update
sudo apt install python3 python3-pyqt6 python3-pil python3-sane python3-opencv python3-numpy python3-pypdf sane-utils tesseract-ocr tesseract-ocr-deu tesseract-ocr-eng
```
