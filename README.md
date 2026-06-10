<div align="center">

<img src="images/icon.svg" alt="GPS Stadtradeln-Tracker Logo" width="120" height="120" style="margin-bottom: 15px;">

# 🚴‍♂️ Stadtradeln GPS Tracker

**Smarte Fahrtenanalyse & Stadtradeln-Eingabehilfe aus GPX, KML, CSV und JSON**

[![Live App](https://img.shields.io/badge/Open_Web_App-006400?style=for-the-badge&logo=appveyor)](https://basecore.github.io/stadtradeln-tracker/)
[![AI Generated](https://img.shields.io/badge/AI_Generated-Perplexity-20B8D9?style=for-the-badge&logo=google)](https://www.perplexity.ai/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/basecore/stadtradeln-tracker)
[![Version](https://img.shields.io/badge/Version-27.2-c1ff00?style=for-the-badge)](https://github.com/basecore/stadtradeln-tracker)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

Eine webbasierte App zur lokalen Auswertung deiner Fahrradfahrten während der **Stadtradeln-Kampagne**. Lade deine GPS-Daten hoch, definiere den Aktionszeitraum und erhalte sofort kopierfertige Einträge für die offizielle Stadtradeln-Plattform – komplett ohne Cloud, ohne Server.

</div>

---

## 🖼️ Vorschau

**Desktop Ansicht** (Upload & Stadtradeln-Einträge):
<p align="center">
  <img src="images/screenshot_desktop_1.png" alt="Desktop Ansicht – Upload & Übersicht" width="49%">
  <img src="images/screenshot_desktop_2.png" alt="Desktop Ansicht – Stadtradeln-Einträge" width="49%">
</p>

**Smartphone Ansicht** (Optimierte mobile Oberfläche):
<p align="center">
  <img src="images/screenshot_mobile_1.png" alt="Mobile Ansicht – Start" width="32%">
  <img src="images/screenshot_mobile_2.png" alt="Mobile Ansicht – Einträge" width="32%">
  <img src="images/screenshot_mobile_3.png" alt="Mobile Ansicht – Optionen" width="32%">
</p>

> 📸 *Screenshots folgen nach dem ersten Release.*

---

## ✨ Was ist neu? (V27.2)

- **localStorage-Persistenz:** Stadtradeln-Zeitraum, Nachtrag-Ende, Min.-Distanz und alle Expertenoptionen werden automatisch gespeichert und beim nächsten Öffnen sofort geladen.
- **First-Run-Assistent:** Beim allerersten Öffnen erscheint ein freundlicher Dialog zur Eingabe des Stadtradeln-Zeitraums – damit du sofort starten kannst.
- **Reset-Button:** Alle gespeicherten Einstellungen lassen sich mit einem Klick auf die Standardwerte zurücksetzen.
- **GitHub Pages Ready:** Die App läuft vollständig im Browser, kein Backend nötig.

---

## 🚀 Hauptfunktionen

### 🔒 100% Lokal & Privat
- **Lokale Verarbeitung im Browser:** Keine Cloud, kein Server. Deine GPS-Daten verlassen dein Gerät zu keinem Zeitpunkt.
- **Automatisches Speichern:** Stadtradeln-Zeitraum und alle Einstellungen werden via `localStorage` dauerhaft gespeichert.

### 📥 Flexibler Import
- **Multi-Format-Support:** GPX, CSV, KML/KMZ und JSON (Google Timeline) werden alle unterstützt.
- **Drag & Drop:** Dateien einfach auf die Upload-Zone ziehen – auch mehrere gleichzeitig.
- **Grobe GPS-Tracks:** Optionaler Modus für ungenau aufgezeichnete Routen (z. B. aus Routenplanern).

### 📋 Stadtradeln-Eingabehilfe
- **Automatische Filterung:** Nur Fahrten im eingestellten Aktionszeitraum + Nachtragszeitraum werden berücksichtigt.
- **Kopierfertige Einträge:** Jeder Eintrag ist mit einem Klick für die Stadtradeln-Plattform kopierbereit.
- **Tageszusammenfassung:** Optional werden mehrere Fahrten eines Tages zu einem Eintrag zusammengefasst.
- **CSV-Export:** Alle Einträge als CSV exportieren für eigene Auswertungen.

### 📊 Analyse & Visualisierung
- **KPI-Übersicht:** Gesamtkilometer, Fahrten, aktive Tage und eingesparte CO₂-Menge auf einen Blick.
- **Wochen-Diagramm:** Balkendiagramm der gefahrenen Kilometer pro Stadtradeln-Woche.
- **Interaktive Karte:** Alle Routen auf einer OpenStreetMap-Karte (Expertenmodus).
- **Detaillierte Fahrtenansicht:** Jede Fahrt mit Metadaten, Notizen und Segmentierungsmöglichkeit.

### ⚙️ Expertenmodus
- **GPS-Filter:** Max. Geschwindigkeit, Sprungdistanz, Pausendauer und Min. Fahrtdistanz konfigurierbar.
- **Manuelle Segmentierung:** Fahrten in Transportmittel-Segmente unterteilen (Fahrrad, zu Fuß, Auto, Bahn).
- **Routenbeschreibungen:** Automatische Erstellung von Routenbeschreibungen pro Fahrt.

---

## 📂 Unterstützte Formate

| Format | Beschreibung |
|--------|-------------|
| 📍 `.gpx` | GPS Exchange Format – Standard für GPS-Tracker |
| 📍 `.kml` / `.kmz` | Keyhole Markup Language – z. B. Google Maps Export |
| 📍 `.csv` | Kommaseparierte Tabelle mit Datum und Distanz |
| 📍 `.json` | Google Timeline / eigene Backup-Dateien |

> 💡 **Tipp:** Über den JSON-Backup-Export kannst du alle Fahrtdaten inkl. Einstellungen sichern und auf anderen Geräten wiederherstellen.

---

## ⚙️ Einrichtung & Bedienung

**Erstmalige Einrichtung:**
1. Öffne die [Web App](https://basecore.github.io/stadtradeln-tracker/)
2. Der **First-Run-Assistent** fragt automatisch nach deinem Stadtradeln-Zeitraum
3. Startdatum, Enddatum, Nachtrag-Ende und minimale Distanz eingeben & speichern

**Dein täglicher Workflow:**
1. GPS-Tracking während der Stadtradeln-Kampagne aufzeichnen (z. B. mit *GPSLogger* oder *Komoot*)
2. Routen-Datei(en) in die App laden (Drag & Drop oder Upload-Button)
3. Einträge prüfen – jede Fahrt erscheint als kopierfertiger Stadtradeln-Eintrag
4. Einträge einzeln oder alle auf einmal in die Stadtradeln-Plattform übertragen
5. Optional: JSON-Backup für spätere Nutzung exportieren

---

## 🧭 Datenquellen & GPS-Aufzeichnung

<details>
<summary><b>Option A: GPSLogger (Android) – Empfohlen</b></summary>

**GPSLogger** ist kostenlos, open-source und ideal für präzise Fahrradaufzeichnungen: [gpslogger.app](https://gpslogger.app/)

**Empfohlene Einstellungen für Stadtradeln:**
- *Dateiformat:* GPX
- *Neue Datei erstellen:* Täglich oder manuell
- *Aufzeichnungsintervall:* 5–10 Sekunden
- *Genauigkeit:* 30–50 Meter
- *Nur aufzeichnen wenn bewegt:* Aktiviert

</details>

<details>
<summary><b>Option B: Komoot / Strava Export</b></summary>

1. Fahrt in Komoot oder Strava aufzeichnen
2. In der App: Aktivität öffnen → **GPX exportieren**
3. GPX-Datei in den Stadtradeln Tracker hochladen

</details>

<details>
<summary><b>Option C: Google Maps Timeline (JSON)</b></summary>

1. Öffne die **Google Maps App** auf deinem Smartphone
2. Tippe auf dein Profilbild → **"Deine Zeitachse"**
3. Drei-Punkte-Menü → **"Standort- und Datenschutzeinstellungen"**
4. **"Zeitachsendaten exportieren"** → JSON-Datei speichern
5. JSON-Datei in den Stadtradeln Tracker hochladen

</details>

<details>
<summary><b>Option D: Google Takeout (KML)</b></summary>

1. Öffne **[Google Takeout](https://takeout.google.com/)**
2. Nur **"Zeitachse"** auswählen → Dateiformat **KML** wählen
3. Export erstellen, ZIP entpacken, KML-Datei hochladen

</details>

---

## 🛠️ Technischer Hintergrund

- **Frontend:** Vanilla JavaScript, HTML5, CSS3 (kein Framework-Overhead)
- **Maps:** [Leaflet.js](https://leafletjs.com/) mit OpenStreetMap-Tiles
- **Charts:** [Chart.js](https://www.chartjs.org/)
- **Speicher:** Browser `localStorage` (Offline-First, keine Cloud)
- **Architektur:** Single-Page-App, vollständig clientseitig
- **Hosting:** GitHub Pages (statisch, kein Backend)

---

## 🌐 Selbst hosten (GitHub Pages)

1. Repository forken: [github.com/basecore/stadtradeln-tracker](https://github.com/basecore/stadtradeln-tracker)
2. In den Repository-Settings → **Pages** → Branch `main` / `/ (root)` aktivieren
3. Fertig – die App läuft unter `https://DEINNAME.github.io/stadtradeln-tracker/`

---

## 📄 Lizenz

Dieses Projekt steht unter der [MIT Lizenz](LICENSE).

---

<div align="center">
  <sub>🤖 <i>Dieses Projekt, die Code-Architektur und die Dokumentation wurden mit KI-Unterstützung (Perplexity AI) erstellt, erweitert und optimiert.</i></sub><br><br>
  <sub>Made with 🚴‍♂️ for Stadtradeln participants everywhere.</sub>
</div>
