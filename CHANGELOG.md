# Changelog

## Version 3.4 – 24.11.2026
- Besser: Meldungen im Cast-Fenster sind gross und gut lesbar und nennen den Grund samt Tipp für das Galaxy Tab
- Neu: Tipp bei der Live-Ansicht: Beamer-Ansicht (2. Gerät) auf dem Handy öffnen und per Smart View spiegeln, so sehen die Schüler QR-Code und Frage, du behältst den Lehrerbereich

## Version 3.3 – 23.11.2026
- Neu: Gemeinsamer KI-Zugang (Mistral). «Mit KI erstellen» funktioniert auch ohne eigenen Schlüssel im Konto, mit Tageslimit. Eigene Schlüssel haben Vorrang

## Version 3.2 – 23.11.2026
- Neu: In ⚙️ Einstellungen (nur Lehrerkonto) gibt es «Google Drive»: «Jetzt in Drive sichern» legt deine Klassen und Vorlagen als Datei (.json) im Drive-Ordner «Teaching Cockpit Backups / Lightning» ab. Eigener Zielordner wählbar, optionale Erinnerung beim Öffnen (höchstens 1× pro Woche). Laufende Sitzungen und Schülerantworten sind nicht enthalten
- Neu, nur für den Besitzer: «Code dieser App sichern» (ZIP in Drive) mit optionaler Erinnerung
- Neue Datei drive-backup.js (gemeinsamer Baustein)

## Version 3.1 – 23.11.2026
- Neu: Fragetyp «📏 Selbsteinschätzung»: mehrere Themen auflisten (1–8), jede Person schätzt jedes Thema auf 5 Stufen ein (sehr sicher … gar nicht). Ergebnis pro Thema als farbiger Balken mit Durchschnitt, dazu «Schwächstes Thema». Auch im Fenster «Mit KI erstellen» wählbar.
- Neu: Anmeldung mit Kästchen «Angemeldet bleiben» (Standard an). Zusätzlich bittet die App den Browser, die Anmeldung dauerhaft zu speichern (hilft auf dem Tablet mit Chrome).
- Keine Änderung an den Firebase-Regeln nötig

## Version 3.0 – 23.11.2026
- Neu: «⚙️ Einstellungen» oben rechts (nur angemeldete Lehrperson, nicht in der Demo): KI-Schlüssel eintragen und «Zuerst fragen» wählen. Gleiches Lehrerkonto wie Sek Planer und Grammatik Trainer, die Schlüssel gelten überall.
- Im KI-Fenster steht nach jeder Antwort, welcher Anbieter und welches Modell geantwortet hat und wie lange es dauerte
- Keine Änderung an den Firebase-Regeln nötig

## Version 2.9 – 23.11.2026
- «Mit KI erstellen», Satz-Korrektur: Die KI baut so viele Fehler ein, wie der Wunsch verlangt (vorher immer genau einen)

## Version 2.8 – 23.11.2026
- Fix: «Mit KI erstellen» meldete bei Satz-Korrektur «keine brauchbaren Fragen», wenn die KI keinen Fragetext mitlieferte. Fehlt er, wird ein passender Auftrag ergänzt. Bei einer unlesbaren Antwort steht jetzt der Anfang der KI-Antwort in der Meldung.

## Version 2.7 – 23.11.2026
- «Mit KI erstellen»: Voreinstellung sind jetzt 3 Fragen (statt 5)

## Version 2.6 – 23.11.2026
- Neu: Im Fenster «Mit KI erstellen» gibt es unter den Fragen «Änderung wünschen» (z. B. «Nr. 3 schwieriger», «nur Richtig-Falsch», «gib mir 10»). Die KI überarbeitet die ganze Liste, beliebig oft.
- Keine Änderung an den Firebase-Regeln nötig

## Version 2.5 – 23.11.2026
- Neu: «✨ Diese Frage mit KI ausfüllen» direkt unter dem Fragefeld (nur Lehrperson). Wunsch eintippen, die KI füllt genau diese eine Frage samt Lösung passend zum gewählten Fragetyp aus. Danach prüfen und ändern.
- «Mit KI erstellen» kann jetzt auch Lückentext und Zuordnen und bis zu 15 Fragen auf einmal
- Schneller: zuerst die schnellen Modelle (Claude Haiku, Gemini Flash ohne Denkphase, Mistral Small); im Fenster steht, welcher Anbieter gerade arbeitet; ein hängender Anbieter wird nach 45 Sekunden übersprungen
- Keine Änderung an den Firebase-Regeln nötig

## Version 2.4 – 23.11.2026
- Neu: «✨ Mit KI erstellen» im Lehrerbereich. Wunsch eintippen, die KI schlägt Fragen vor (alle Typen ausser Lückentext und Zuordnen). Jede Frage kann ins Formular geladen oder als Vorlage gespeichert werden, oder alle zusammen als Vorlagen. Benutzt den eigenen KI-Schlüssel aus dem Konto (wie im Sek Planer), nichts läuft über einen fremden Zwischenserver. Nicht in der Demo.
- Keine Änderung an den Firebase-Regeln nötig

## Version 2.3 – 23.11.2026
- Neu: Sessions und Antworten bleiben 30 Tage gespeichert (vorher 24 Stunden), danach werden sie automatisch gelöscht. «Beendet» zeigt die letzten 30 Tage, nach Datum gruppiert.
- Neu: Der Cast-Knopf erscheint nur für die angemeldete Lehrperson (nicht für Schüler, nicht in der Beamer-Ansicht).
- Fix: «Session konnte nicht gestartet werden» bei sechsstelligen Codes, solange die Firebase-Regeln nur vierstellige erlauben; klare Fehlermeldung bei verweigerten Regeln.
- Keine Änderung an den Firebase-Regeln nötig

## Version 2.2 – 22.11.2026
- Neu: «🔗 Link kopieren» neben dem Code (Link mit Code für Teams oder Chat) und die kurze Adresse als Text, falls ein Schüler den QR-Code nicht scannen kann
- Keine Änderung an den Firebase-Regeln nötig

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
