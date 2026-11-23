# Lightning – Live-Checks & Exit-Tickets

Live-App: https://novarion-desk.github.io/lightning/

Warm-up, Zwischencheck und Exit-Ticket im Unterricht: Die Lehrperson startet eine Frage,
die Schüler/innen scannen den QR-Code (ohne Login) und antworten mit dem Handy oder iPad.

## Ansichten

| Ansicht | Aufruf | Login |
|---|---|---|
| Lehrperson | `./` | Lehrpersonen-Konto (gleiches Firebase-Konto wie die anderen Apps) |
| Schüler/innen | `./?code=1234` oder Code eingeben | keines (geheimer Geräteschlüssel) |
| Beamer (2. Gerät) | `./?beamer=1234` | Lehrpersonen-Konto |
| Projektionsmodus | Knopf «📽️ Projektionsmodus» im Dashboard – Tablet zeigt nur QR, Frage und anonyme Ergebnisse, mit Steuerleiste | – |
| Demo | `./?demo` | keines – nichts wird gespeichert, simulierte Klasse |

## Fragetypen

Kurzantwort · Multiple Choice · Ampel (1–4 + Rückfrage) · Satz-Korrektur · Reihenfolge · Richtig/Falsch · Wortwolke · Zahl/Schätzung · Lückentext · Zuordnen

Zu jeder Frage kann ein Bild hinzugefügt werden. Ergebnisse lassen sich als CSV exportieren (öffnet in Excel/Numbers).

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
- Lösungen liegen privat bei der Lehrperson (`lightningTeachers/<uid>/solutions`); die automatische Rückmeldung berechnet das Gerät der Lehrperson.
- Feedback (✅/⚠️/❌, Kommentar) sieht nur der betroffene Schüler auf seinem Gerät. Nachbessern ist nur nach ⚠️/❌ und nur mit Erlaubnis der Lehrperson möglich – auch das prüft die Datenbank.
- Sessions und Antworten werden 30 Tage nach dem Start automatisch gelöscht (beim nächsten Login der Lehrperson).
- Nur Vornamen oder Kürzel speichern.

## Feedback zur App
Der Knopf «📝 App-Feedback» öffnet ein externes, anonymes Formular bei Tally (Fehler, Wünsche). Nur dann werden Angaben gesendet – zusammen mit App-Name, Version und Gerätetyp. Namen werden nicht abgefragt. Mit den Kommentaren an Schüler hat das nichts zu tun.
