# Changelog

## Version 2.1 – 22.11.2026
- Neu: 📺-Knopf unten links «Auf Bildschirm senden»: Cast-Bildschirm (Chrome) oder «Als Fenster öffnen» für einen zweiten Bildschirm. «Getrennt»: Bildschirm zeigt die Beamer-Ansicht (Projektionsmodus 📽️ einschalten), du siehst weiter dein Dashboard. «Gleich»: dasselbe wie du. Nichts davon läuft über Firebase

## Version 2.0 – 22.11.2026
- Neu: 🔤 Lückentext. Wörter in eckige Klammern setzen, z. B. «I [have] lived here [for/since] three years.»; Schüler setzen ein, automatische Rückmeldung («1 von 2 Lücken richtig»), Auswertung pro Lücke am Beamer
- Neu: 🔗 Zuordnen (2–8 Paare, «links = rechts»); Schüler wählen pro Begriff aus einer Liste, Auswertung pro Paar
- Neu: 🖼️ Bild zur Frage (bei jedem Fragetyp; wird verkleinert und in der Frage gespeichert, auch in Vorlagen). Sichtbar bei Schülern, Beamer und Lehrperson
- Neu: «❓ Offene Fragen sammeln»: Vorlage für anonyme Rückfragen (Kurzantwort, Namen am Beamer bleiben aus)
- Bereits vorhanden (jetzt in der Übersicht der Fragetypen ergänzt): Wortwolke, Zahl/Schätzung, Richtig/Falsch, Zeitlimit mit Countdown, CSV-Export
- Keine Änderung an den Firebase-Regeln nötig

## Version 1.9.1 – 21.11.2026
- Sicherheit: Der Code für Schüler ist neu 6-stellig (statt 4), damit er schwerer zu erraten ist. Ältere 4-stellige Codes funktionieren zum Beitreten weiter. Sonst keine Änderung.

## Version 1.9 – 21.11.2026
- Neu: Zurück-Geste / Zurück-Taste schliesst offene Fenster bzw. geht von der laufenden Frage zurück zur Startansicht (die Frage läuft weiter), statt die App zu schliessen.

## v1.8 – 21.11.2026
- Neuer Knopf «📝 App-Feedback» in der Kopfzeile: öffnet ein anonymes Formular für Fehler und Wünsche zur App (nicht zu verwechseln mit dem Kommentar an Schüler). Version und Gerät werden automatisch mitgegeben; es werden keine Namen abgefragt.

## v1.7 – 19.11.2026
- ↩︎ Zurückgeben: Antwort an einen Schüler zum Überarbeiten zurückgeben (mit optionalem Kommentar). Er sieht seine bisherige Antwort im Feld und darf sie ändern – auch wenn die Eingabe für alle gesperrt ist. Danach «✏️ überarbeitet».
- ↶ Rückgängig in der Kopfzeile: Bewertung, Kommentar, Zurückgeben, Antwort löschen, Frage beenden/löschen, Sperren, Zeitlimit, Anwesenheit und Einstellungen – solange die App offen ist. Nach dem Löschen zusätzlich «Rückgängig» im Hinweis.
- «Heute beendet»: 🗑 löscht eine Frage mit allen Antworten sofort.

## v1.6 – 19.11.2026
- Klick aufs ⚡-Logo oder «← Übersicht» führt zur Startseite, ohne die Frage zu beenden (sie bleibt in «Deine Fragen» offen).
- «👤 Namen am Beamer» (Standard AUS): zeigt die Namen auf den Antwortkarten und beim Spotlight am Beamer. Auch in der Leiste des Projektionsmodus.

## v1.5 – 19.11.2026
- QR-Code antippen → bildschirmfüllend mit Code und Adresse (Dashboard, Projektionsmodus, Beamer-Ansicht). Antippen oder Esc schliesst.
- «Deine Fragen» auf der Startseite: laufende Fragen (live auf allen Geräten, «Öffnen»/«Beenden») und heute beendete («Ergebnisse», «Wieder öffnen»). Eine auf dem Tablet gestartete Frage erscheint sofort auch am Mac. Gelöscht wird weiterhin automatisch nach 24 Stunden.
- Beendete Frage im Dashboard: Hinweis «Beendet» mit «Wieder öffnen».

## v1.4 – 19.11.2026
- Anwesenheit: Nach der Klassenwahl alle Namen antippen, wer fehlt (grau). Schüler sehen im Namen-Menü nur die Anwesenden, der Abgabestatus zählt nur sie («9 / 12 abgegeben · 2 abwesend»). Die Auswahl gilt heute für diese Klasse (pro Gerät), danach wieder alle.
- ⚙️ Einstellungen während der Frage: Anwesenheit anpassen (z. B. Zuspätkommende), Nachbessern, ⭐-Hinweis, Namen sichtbar, Zeitlimit neu setzen oder entfernen. «Nachbessern» ist aus der Knopfleiste in dieses Fenster gewandert.
- Demo: Klasse mit 2 Abwesenden.

## v1.3 – 19.11.2026
- Multiple Choice: 2–8 Optionen, richtige Antwort(en) markierbar, Mehrfachauswahl.
- Reihenfolge: 3–10 Elemente, im Formular verschiebbar.
- Kurzantwort und Satz-Korrektur: optionale Musterlösung (mehrere möglich).
- Neue Typen: ⚖️ Richtig/Falsch, ☁️ Wortwolke (1, bis 2, 3 oder 5 Begriffe), 🔟 Zahl/Schätzung (mit Verteilung, Median, Toleranz, Einheit).
- Automatische Rückmeldung, sobald eine Lösung hinterlegt ist (bei Reihenfolge z. B. «4 von 5 an der richtigen Stelle»). Die Lösung bleibt privat, bis «💡 Lösung zeigen» gedrückt wird – dann erscheint sie am Beamer und bei den Schülern.
- Vorlagen und KI-Import kennen alle neuen Typen und Lösungen.

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
