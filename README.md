# Lightning – Live-Checks & Exit-Tickets

Live-App: https://novarion-desk.github.io/lightning/

Warm-up, Zwischencheck und Exit-Ticket im Unterricht: Die Lehrperson startet eine Frage,
die Schüler/innen scannen den QR-Code (ohne Login) und antworten mit dem Handy oder iPad.

## Ansichten

| Ansicht | Aufruf | Login |
|---|---|---|
| Lehrperson | `./` | Lehrpersonen-Konto (gleiches Firebase-Konto wie die anderen Apps) |
| Schüler/innen | `./?code=1234` oder Code eingeben | keines (unsichtbares anonymes Login) |
| Beamer | `./?beamer=1234` | Lehrpersonen-Konto |

## Fragetypen

Kurzantwort · Multiple Choice · Ampel (1–4 + Rückfrage) · Satz-Korrektur · Reihenfolge

## Aufbau

| Pfad | Inhalt |
|---|---|
| `index.html` | Die ganze App |
| `vendor/` | Firebase, QR-Code, CSS – fest im Repo, keine fremden Server |
| `firestore.rules` | Sicherheitsregeln (Kopie; aktiv sind die Regeln in der Firebase-Konsole) |
| `icons/`, `manifest.webmanifest`, `sw.js` | Installierbar als App |

## Daten & Datenschutz

- Firebase Firestore (Region europe-west6, Zürich), Projekt «Unterrichtscockpit».
- Klassenlisten und Vorlagen liegen privat pro Lehrperson (`lightningTeachers/<uid>`).
- Eine Session (`lightningSessions/<code>`) enthält nur die Frage und die Namen der gewählten Klasse.
- Schüler/innen können nur ihre eigene Antwort schreiben und lesen. Sperre und Timer gelten auch in der Datenbank (Serverzeit).
- Sessions und Antworten werden 24 Stunden nach dem Start automatisch gelöscht (beim nächsten Login der Lehrperson).
- Nur Vornamen oder Kürzel speichern.
