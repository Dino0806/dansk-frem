# 🇩🇰 Dansk Frem

**DE** · [EN](#english)

Eine persönliche Dänisch-Lern-App, die direkt im Browser läuft – ohne Installation, ohne Server, ohne Abo.

---

## Was kann die App?

| Tab | Funktion |
|---|---|
| 🏠 **Hjem** | Niveau-Anzeige (A1–C1), Tages-Challenge, Aktivitätschart (7/30/90 Tage), Streak |
| 💬 **Samtale** | KI-Chat mit Personas (Lars – Kollega, Maja – Veninde, Fri situation) + automatische Fehlerkorrektur |
| ✍️ **Øv** | Texteingabe oder Foto von Handschrift → KI-Korrektur mit korrigiertem Text; Grammatik-Regelkarten & Lückentext-Übungen |
| 🗺️ **Øer** | Sprogøer: Fachvokabular-Inseln per Interview aufbauen, üben (DE→DA), als CSV oder Anki exportieren |
| 📋 **Log** | Fejllog: alle Fehler gesammelt, gefiltert, exportierbar; Anki-Kartenexport; 🎯 Recall-Test (Tagestest & Schwächentest) |
| 📓 **Noter** | Freie Notizen mit Zeitstempel + KI-Korrektur auf Wunsch |

---

## Schnellstart

### Lokal
1. `index.html` herunterladen
2. Datei im Browser öffnen (Doppelklick oder Drag & Drop)
3. Beim ersten Start: API-Key eingeben (`sk-ant-...`)
4. Loslegen 🎉

### Gehostet via GitHub Pages
**Schritt 1** – GitHub-Konto erstellen: [github.com/signup](https://github.com/signup)

**Schritt 2** – Neues Repository erstellen
1. „+" → „New repository" → Name z. B. `dansk-frem`
2. „Public" auswählen → „Create repository"

**Schritt 3** – `index.html` hochladen
- „Add file" → „Upload files" → `index.html` hochladen → Commit

**Schritt 4** – GitHub Pages aktivieren
- Repository → „Settings" → „Pages" → Source: `main`, `/ (root)` → „Save"

Nach 1–2 Minuten erreichbar unter:
```
https://DEIN-GITHUB-NAME.github.io/dansk-frem/
```

**Schritt 5** – Als App auf dem Handy speichern

*iPhone (Safari):* Teilen-Button → „Zum Home-Bildschirm"

*Android (Chrome):* Drei-Punkte-Menü → „Zum Startbildschirm hinzufügen"

---

## API-Key & Zugang

Beim ersten Öffnen erscheint ein Eingabefenster für den Anthropic API-Key. Der Key wird nur lokal im Browser gespeichert und direkt an Anthropic gesendet.

Einen Key erstellen: [console.anthropic.com](https://console.anthropic.com)

> **Tipp:** Unter console.anthropic.com → Settings → Limits ein monatliches Budget-Limit setzen (z. B. $15–20).

### Admin-Modus (unbegrenzte Nutzung)
```
https://DEIN-GITHUB-NAME.github.io/dansk-frem/?admin=DEIN-PASSWORT
```
Das Passwort ist in der Datei unter `ADMIN_PASS` festgelegt. Ohne diesen Parameter gilt ein tägliches Limit von 50 Anfragen pro Browser.

---

## Anki-Export

| Typ | Beschreibung |
|---|---|
| **Kontext** | 8 Felder: Satz_DA, Wort, IPA, Satz_DE, Wort_DE, Wortart, Eselsbrücke, Grammatik – Audio nachrüstbar |
| **Lückentext** | Aus dem Fehlerlog: Satz mit Lücke + Grammatikhinweis |
| **Sprogø-Satz** | Dänischer Satz → deutsche Übersetzung |

---

## Cloud-Sync

Einstellungen → ☁️ Cloud-Sync → „Log ind med Google"

Daten (Fehlerlog, Notizen, Statistik, Sprogøer) werden verschlüsselt in Firebase gespeichert und geräteübergreifend synchronisiert.

---

## Datenschutz

- Alle Daten lokal im Browser (`localStorage`)
- Mit Cloud-Sync: verschlüsselt in Firebase, verknüpft mit Google-Konto
- Keine Werbung, kein Tracking, keine Drittanbieter-Analytics

---

## Technische Details

| | |
|---|---|
| **Stack** | Reines HTML/CSS/JS – eine einzige Datei |
| **KI-Modell** | `claude-sonnet-4-20250514` via Anthropic API |
| **Libraries** | sql.js 1.10.2, JSZip 3.10.1 |
| **Auth/Sync** | Firebase (optional) |

---
---

# English

<a name="english"></a>

**[DE](#)** · EN

A personal Danish learning app that runs directly in the browser – no installation, no server, no subscription.

---

## What can the app do?

| Tab | Function |
|---|---|
| 🏠 **Hjem** | Level display (A1–C1), daily challenge, activity chart (7/30/90 days), streak |
| 💬 **Samtale** | AI chat with personas (Lars – colleague, Maja – friend, free situation) + automatic error correction |
| ✍️ **Øv** | Text input or photo of handwriting → AI correction with corrected text; grammar rule cards & gap-fill exercises |
| 🗺️ **Øer** | Sprogøer: build domain-specific vocabulary islands via interview, practice (DE→DA), export as CSV or Anki |
| 📋 **Log** | Fejllog: all errors collected, filtered, exportable; Anki card export; 🎯 Recall test (daily test & weakness test) |
| 📓 **Noter** | Free notes with timestamp + AI correction on request |

---

## Quick Start

### Local
1. Download `index.html`
2. Open in browser (double-click or drag & drop)
3. On first launch: enter your API key (`sk-ant-...`)
4. Start learning 🎉

### Hosted via GitHub Pages
**Step 1** – Create a GitHub account: [github.com/signup](https://github.com/signup)

**Step 2** – Create a new repository
1. „+" → „New repository" → name e.g. `dansk-frem`
2. Select „Public" → „Create repository"

**Step 3** – Upload `index.html`
- „Add file" → „Upload files" → upload `index.html` → Commit

**Step 4** – Enable GitHub Pages
- Repository → „Settings" → „Pages" → Source: `main`, `/ (root)` → „Save"

Available after 1–2 minutes at:
```
https://YOUR-GITHUB-NAME.github.io/dansk-frem/
```

**Step 5** – Add to home screen

*iPhone (Safari):* Share button → „Add to Home Screen"

*Android (Chrome):* Three-dot menu → „Add to Home Screen"

---

## API Key & Access

On first launch, a dialog asks for your Anthropic API key. The key is stored only locally in your browser and sent directly to Anthropic.

Get a key at: [console.anthropic.com](https://console.anthropic.com)

> **Tip:** Set a monthly budget limit at console.anthropic.com → Settings → Limits (e.g. $15–20).

### Admin mode (unlimited usage)
```
https://YOUR-GITHUB-NAME.github.io/dansk-frem/?admin=YOUR-PASSWORD
```
The password is defined in the file under `ADMIN_PASS`. Without this parameter, a daily limit of 50 requests per browser applies.

---

## Anki Export

| Type | Description |
|---|---|
| **Kontext** | 8 fields: Satz_DA, Wort, IPA, Satz_DE, Wort_DE, Wortart, Eselsbrücke, Grammatik – audio can be added later |
| **Lückentext** | From error log: sentence with gap + grammar note |
| **Sprogø sentence** | Danish sentence → German translation |

---

## Cloud Sync

Settings → ☁️ Cloud-Sync → „Log ind med Google"

Data (error log, notes, stats, Sprogøer) is stored encrypted in Firebase and synced across all devices.

---

## Privacy

- All data stored locally in the browser (`localStorage`)
- With Cloud-Sync: encrypted in Firebase, linked to your Google account
- No ads, no tracking, no third-party analytics

---

## Technical Details

| | |
|---|---|
| **Stack** | Pure HTML/CSS/JS – a single file |
| **AI Model** | `claude-sonnet-4-20250514` via Anthropic API |
| **Libraries** | sql.js 1.10.2, JSZip 3.10.1 |
| **Auth/Sync** | Firebase (optional) |

---

*Built with Claude (Anthropic) · Runs locally in the browser · No registration required*
