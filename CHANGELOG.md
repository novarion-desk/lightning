# Changelog

## v1.2 – 19.11.2026
- Feedback an Schüler: ✅ Richtig, ⚠️ Fast, ❌ Noch nicht – erscheint sofort auf dem Gerät des Schülers (nicht am Beamer), mit kurzer Vibration.
- 💬 Kurzkommentar (max. 120 Zeichen) mit Textbausteinen; eigene Bausteine speicherbar.
- Schalter «Nachbessern erlaubt» beim Start und während der Frage: Schüler dürfen nach ⚠️/❌ korrigieren; die Karte zeigt dann «✏️ nachgebessert». Ohne Erlaubnis ist eine bewertete Antwort gesperrt.
- Optionaler ⭐-Hinweis: Schüler sehen, wenn ihre Antwort anonym am Beamer besprochen wird.
- Sicherheit: Für das Spotlight steht in der Session nur noch ein Hash, nicht mehr der geheime Geräteschlüssel.
- CSV mit Feedback, Kommentar und «nachgebessert»; Demo-Schüler bessern nach Feedback nach.

## v1.1 – 18.11.2026
- Projektionsmodus: Tablet zeigt beim Spiegeln nur QR-Code, Frage und anonyme Ergebnisse; Steuerleiste ohne Namen (Ergebnisse, Sperren, +30s, Spotlight per Tipp auf eine Karte).
- Demo-Version `?demo`: ohne Login, nichts wird gespeichert, simulierte Schülerantworten, Beispielklasse und Vorlagen.

## v1 – 18.11.2026
- Erste Version (Grundlage mit Gemini erstellt, überarbeitet).
- Firestore statt Realtime Database, im gemeinsamen Projekt «Unterrichtscockpit».
- Login für Lehrpersonen; Schüler/innen ohne Login (geheimer Geräteschlüssel).
- Klassenlisten, Vorlagen und Lösungen privat pro Lehrperson.
- Schüler sehen nur ihre eigene Antwort; Sperre/Timer serverseitig erzwungen.
- Lösung bei «Reihenfolge» für Schüler nicht mehr sichtbar.
- Automatisches Löschen nach 24 Stunden, Session nach Neuladen fortsetzen.
- «Gerät weitergeben» für geteilte iPads, Klassen bearbeiten, CSV mit Umlauten.
- Installierbar als App mit eigenem Icon.
