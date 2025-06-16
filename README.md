
# Berechnung Dienstteil 4.30 h Lenkzeit und 1/6 Regelung

Diese Web-App dient der Überprüfung von Lenkzeitüberschreitungen und der Anwendung der sogenannten **1/6-Regelung** für Wendezeiten/Endpunkte im Fahrdienst.

## Funktionen

- Eingabe von:
  - Dienstbeginn und Dienstende
  - Wendezeiten / Endpunkten (max. 20)
  - Stand- und Wartezeiten über 1 Minute (max. 20)

- Automatische Berechnung von:
  - Arbeitszeit
  - Lenkzeit
  - Prüfung der 4:30 h Lenkzeitgrenze
  - Anwendung der 1/6-Regel bei Überschreitung

- Bewertung mit Ampelfarben:
  - ✅ Lenkzeit unter 4:30 h
  - ✅ 1/6-Regel erfüllt
  - ❌ Verstoß bei zu langer Lenkzeit ohne ausreichende Wendezeiten

## Nutzung

1. Öffne die App im Browser:
   ```
   https://<dein-benutzername>.github.io/<dein-repository-name>/
   ```

2. Trage Dienstbeginn und Dienstende ein

3. Gib Wendezeiten (nur ≥ 11 Minuten werden berücksichtigt) und Standzeiten ein

4. Klicke auf **Berechnen**

## PWA-Funktion

Die App kann auf dem Startbildschirm installiert werden (z. B. unter iOS oder Android), wenn sie über HTTPS aufgerufen wird.

## Struktur

- `index.html` – Hauptanwendung
- `manifest.json` – PWA Manifest
- `service-worker.js` – für Offlinebetrieb
- `icon-192.png` / `icon-512.png` – App Icons

---

© 2025 – Erstellt für betriebliche Berechnungen im Linienverkehr
