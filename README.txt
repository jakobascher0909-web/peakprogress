PeakProgress – Handy-App (PWA)

INHALT
- index.html: die App
- manifest.json + sw.js + Icons: Installierbarkeit und Offline-Grundgeruest

WICHTIG
Du kannst index.html am PC direkt öffnen. Für eine echte Installation auf dem Handy als App muss dieser Ordner über eine HTTPS-Adresse erreichbar sein (z. B. GitHub Pages oder Netlify). Nur die HTML-Datei per WhatsApp zu schicken oder lokal zu öffnen reicht für die PWA-Installation nicht.

INSTALLATION NACH DEM HOSTING
Android (Chrome): Website öffnen -> Menü (⋮) -> „App installieren“ oder „Zum Startbildschirm hinzufügen“.
iPhone (Safari): Website öffnen -> Teilen -> „Zum Home-Bildschirm“.

AKTIVITÄTEN IMPORTIEREN
- GPX und TCX: im Browser auslesen, Werte prüfen, dann in PeakProgress speichern.
- Screenshot: optional OCR-Texterkennung. Dafür wird Tesseract.js aus einem CDN geladen; dafür ist Internet nötig. Die Bilddatei wird im Browser verarbeitet. OCR kann Zahlen falsch erkennen, bitte immer kontrollieren.
- FIT: Garmins natives FIT-Format wird in dieser Version noch nicht direkt ausgewertet. Wenn möglich GPX/TCX exportieren oder vorerst einen Screenshot verwenden.

DATENSCHUTZ & DATEN
Die Einträge bleiben im lokalen Browser (localStorage). Exportiere regelmäßig ein JSON-Backup über „Verlauf“. Browserdaten löschen kann lokale Einträge entfernen. Die App verbindet sich nicht automatisch mit Garmin Connect.

Skitage werden nach eindeutigen Kalenderdaten gezählt; mehrere Ski-Aktivitäten am selben Tag zählen daher als ein Skitag.
