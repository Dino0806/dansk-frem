# 🇩🇰 Dansk Frem

Eine persönliche Dänisch-Lern-App, die direkt im Browser läuft – ohne Installation, ohne Server, ohne Abo.

---

## Was kann die App?

| Tab | Funktion |
|-----|----------|
| 🏠 **Hjem** | Niveau-Anzeige (A1–C1), Tages-Challenge, Lerntipps |
| 💬 **Samtale** | KI-Chat mit Personas (Kollege, Chef, Alltag) + Job-Szenarien |
| ✍️ **Skriv** | Texteingabe oder Foto von Handschrift → KI-Korrektur |
| 📖 **Sprog** | Grammatik-Regelkarten & Übungen + Satzbausteine / Phrasebook |
| 📋 **Fejllog** | Alle Fehler gesammelt, gefiltert, exportierbar (CSV, TXT, Anki) |
| 🃏 **Anki** | Flashcard-Generator → Export als echte `.apkg`-Datei |
| 📓 **Noter** | Freie Notizen mit Zeitstempel + KI-Korrektur auf Wunsch |

---

## Voraussetzungen

- Ein **Anthropic API-Key** (kostenlos erstellen unter [console.anthropic.com](https://console.anthropic.com))
- Ein moderner Browser (Chrome oder Edge empfohlen)
- Kosten: ca. **$0,003 pro Gespräch** – ein Budget-Limit in der Anthropic Console wird empfohlen (z. B. $5/Monat)

---

## Schnellstart (lokal)

1. `dansk-laer.html` herunterladen
2. Datei im Browser öffnen (Doppelklick oder per Drag & Drop)
3. Oben rechts auf ⚙️ klicken
4. API-Key eingeben (`sk-ant-api03-...`) und speichern
5. Loslegen 🎉

---

## Hosting via GitHub Pages (empfohlen für Handy-Nutzung)

So wird die App dauerhaft unter einer eigenen URL erreichbar – ideal als Homescreen-App auf dem Handy.

### Schritt 1 – GitHub-Konto erstellen
Falls noch nicht vorhanden: [github.com/signup](https://github.com/signup)

### Schritt 2 – Neues Repository erstellen
1. Auf [github.com](https://github.com) einloggen
2. Oben rechts auf **„+"** → **„New repository"**
3. Name eingeben, z. B. `dansk-frem`
4. **„Public"** auswählen (wichtig für GitHub Pages)
5. **„Create repository"** klicken

### Schritt 3 – Dateien hochladen
1. Im neuen Repository auf **„Add file"** → **„Upload files"**
2. `dansk-laer.html` hochladen
3. Die Datei in `index.html` **umbenennen** (wichtig!)  
   → Datei anklicken → Stift-Icon → oben den Dateinamen auf `index.html` ändern → speichern
4. Auch `README.md` hochladen (optional)

### Schritt 4 – GitHub Pages aktivieren
1. Im Repository auf **„Settings"** (oben in der Menüleiste)
2. Links im Menü: **„Pages"**
3. Unter „Source": **„Deploy from a branch"** auswählen
4. Branch: **`main`**, Ordner: **`/ (root)`**
5. **„Save"** klicken

Nach 1–2 Minuten ist die App erreichbar unter:
```
https://DEIN-GITHUB-NAME.github.io/dansk-frem/
```

### Schritt 5 – Als App auf dem Handy speichern

**iPhone (Safari):**
1. URL im Safari öffnen
2. Teilen-Button (Viereck mit Pfeil) antippen
3. **„Zum Home-Bildschirm"** wählen

**Android (Chrome):**
1. URL in Chrome öffnen
2. Drei-Punkte-Menü oben rechts
3. **„Zum Startbildschirm hinzufügen"**

Die App erscheint dann wie eine native App auf dem Homescreen.

---

## API-Key einrichten (einmalig)

1. App öffnen → ⚙️ antippen
2. API-Key einfügen (`sk-ant-api03-...`)
3. **„Speichern"** tippen

Der Key wird nur lokal im Browser gespeichert (localStorage) und direkt an Anthropic gesendet – er verlässt nicht dein Gerät.

> **Tipp:** Unter [console.anthropic.com](https://console.anthropic.com) → „Settings" → „Limits" ein monatliches Budget-Limit setzen, z. B. $5.

---

## Datenschutz & Datenspeicherung

- Alle Daten (Fehlerlog, Notizen, Statistik, Phrasen) werden **ausschließlich lokal** im Browser gespeichert (`localStorage`)
- Es werden **keine Nutzerdaten** an Server gesendet außer den Nachrichten an die Anthropic API
- Die App läuft vollständig clientseitig – kein Backend, kein Login, keine Cloud

---

## Technische Details

| | |
|-|-|
| Technologie | Reines HTML/CSS/JS (eine einzige Datei) |
| KI-Modell | `claude-sonnet-4-20250514` via Anthropic API |
| Externe Libraries | sql.js 1.10.2, JSZip 3.10.1 (für Anki-Export) |
| Offline-fähig | Nein (benötigt Internetverbindung für KI-Funktionen) |
| Datenspeicherung | `localStorage` im Browser |

---

*Erstellt mit Claude (Anthropic) · Läuft lokal im Browser · Keine Registrierung erforderlich*
