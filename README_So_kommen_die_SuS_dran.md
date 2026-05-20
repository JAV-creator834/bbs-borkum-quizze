# Quizze online stellen – Anleitung für JAV

Die Quiz-HTML-Dateien in diesem Ordner müssen **auf einem Webserver liegen**, damit sie für die SuS funktionieren. Eine HTML-Datei per E-Mail oder Cloud-Link zu verschicken klappt **nicht** – Browser blockieren JavaScript in lokal heruntergeladenen HTML-Dateien aus Sicherheitsgründen.

Empfohlene Lösung: **GitHub Pages** (kostenlos, dauerhaft, einmalig einrichten).

---

## Einmaliges Setup – GitHub-Account + Repository (~ 10 Min)

### 1. Account erstellen

1. <https://github.com/signup> öffnen
2. Dauerhaft genutzte E-Mail-Adresse + Passwort wählen
3. Benutzername wählen (Kleinbuchstaben, keine Leerzeichen). Vorschlag: `janet-vogt-bbs` o. ä.
4. E-Mail bestätigen, kostenlosen Plan wählen

### 2. Repository anlegen

1. Oben rechts **+** → **New repository**
2. Name: `bbs-borkum-quizze`
3. Beschreibung: „Interaktive Quizze BBS Borkum – Lehrkraft JAV"
4. **Public** lassen (Pages funktioniert sonst nicht im Free-Plan)
5. Haken bei **Add a README file**
6. **Create repository**

### 3. GitHub Pages aktivieren

1. Im Repository oben **Settings** anklicken
2. Linke Seitenleiste: **Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** + Ordner: **/ (root)** → **Save**
5. Nach 1–2 Min erscheint die URL: `https://DEIN-USERNAME.github.io/bbs-borkum-quizze/`

---

## Jedes neue Quiz hochladen (~ 1 Min)

1. Repository öffnen
2. **Add file** → **Upload files**
3. HTML-Datei per Drag & Drop ablegen
4. **Commit changes**
5. URL bilden: `https://DEIN-USERNAME.github.io/bbs-borkum-quizze/Quiz_DATEINAME.html`

---

## Die Quiz-URLs verteilen

Möglichkeiten, die URL an SuS zu bringen:

- **QR-Code an die Tafel projizieren** – Generator: <https://www.qrcode-generator.de/>
- **Per Mail / WhatsApp / IServ** verschicken – jetzt als URL, nicht mehr als Datei
- In Moodle / IServ / ILIAS als externen Link einfügen

---

## Lehrkraft-Modus

URL um `?modus=lehrer` ergänzen:
```
https://DEIN-USERNAME.github.io/bbs-borkum-quizze/Quiz_Einheit_8_Recht_Ordnung_Versand.html?modus=lehrer
```
→ alle Lösungen direkt sichtbar (für Plenum-Auswertung).

---

## Datenschutz – wichtiger Hinweis

**Das Repository ist öffentlich** – jede:r mit der URL sieht die Quiz-Inhalte. Das ist für **Quizfragen unkritisch** (keine SuS-Daten, keine Klassennamen, keine Noten enthalten).

**NICHT** in das Repository legen:
- Klassenarbeiten / Musterlösungen
- Schüler:innen-Mappen oder Reflexionsbögen
- Bewertungsrubriken mit echten Namen
- Personalakten oder andere personenbezogene Daten

Für diese sensiblen Dokumente bleibt dein lokaler Projektordner zuständig.

---

## Warum nicht E-Mail-Anhang?

| Übertragung | Funktioniert? | Warum |
|---|---|---|
| E-Mail-Anhang | ❌ | Lokale HTML → Browser blockiert JavaScript |
| WhatsApp / iMessage | ❌ | Mobile Browser öffnen lokale HTML nicht zuverlässig |
| Dropbox / iCloud / OneDrive | ❌ | Bieten HTML nur zum Download an |
| GitHub Pages / Netlify | ✅ | Echte URL, Browser lädt wie normale Website |

---

*Anleitung für: Janet Vogt (JAV) · BBS Borkum · Stand 2026-05-20*
