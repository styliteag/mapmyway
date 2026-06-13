---
title: Changelog
description: What changed in each MapMyWay release.
---

# Changelog

## 1.2.4 — 2026-06-14


**Deutsch**

- Ortsverwaltung: Fehler beim Löschen oder Zusammenführen eines Orts werden jetzt als Hinweis angezeigt, statt die Ansicht stillschweigend zu schließen


**English**

- Place management: errors when deleting or merging a place are now surfaced as a banner instead of silently dismissing the screen

## 1.2.3 — 2026-06-12


**Deutsch**

- Behebt einen Absturz beim Wechsel in den Hintergrund während der Timeline-Verarbeitung
- Datenbank-Zugriffe werden vor dem Schlafenlegen der App jetzt sauber abgeschlossen


**English**

- Fixes a crash when the app moved to the background during timeline processing
- Database access is now wound down cleanly before the app is suspended

## 1.2.2 — 2026-06-12


**Deutsch**

- Aktualisierte Tracking-Engine (LocoKit2)
- Interne Verbesserungen an Stabilität und Diagnose-Logging


**English**

- Updated tracking engine (LocoKit2)
- Internal stability and diagnostics-logging improvements

## 1.2.1 — 2026-06-12


**Deutsch**

- Kalender: der Tages-Streifen reicht jetzt beliebig weit zurück und folgt Sprüngen über das Kalender-Widget (vorher Limit: 30 Tage)
- Neu: „Unbekannte Orte benennen“ (Einstellungen → Orte) — häufig besuchte Orte ohne Namen, meistbesuchte zuerst; ein Name benennt alle Besuche auf einmal
- Neu: „Was ist neu“-Link im Hilfe-Bereich führt zur vollständigen Änderungsübersicht


**English**

- Calendar: the day strip now reaches arbitrarily far back and follows date-picker jumps (previously limited to 30 days)
- New: "Name Unknown Places" (Settings → Places) — frequently visited spots without a name, most visited first; one name covers all visits at once
- New: "What's New" link in the help section opens the full changelog

## 1.2.0 — 2026-06-12


**Deutsch**

- Neu: „Alte Daten verdichten“ (Einstellungen → Speicher) — dünnt alte Standort-Samples aus und verkleinert die Datenbank um bis zu 60 %, Orte und Routen bleiben vollständig erhalten
- Fahrten ohne erkannte Aktivität zeigen jetzt das richtige Verkehrsmittel statt „Fahrt“
- Doppelt angelegte Orte (z. B. nach Importen) werden automatisch zusammengeführt
- Orts-Statistiken (Besuchszähler, Radius) werden automatisch repariert
- Karte beim Benennen und Bestätigen von Orten ist jetzt zoombar und startet näher am Ort; Vorschläge folgen dem Kartenausschnitt


**English**

- New: "Compact Old Data" (Settings → Storage) — thins out old location samples and shrinks the database by up to 60%, places and routes stay fully intact
- Trips without a detected activity now show the right mode of transport instead of generic "Trip"
- Duplicate places (e.g. after imports) are merged automatically
- Place statistics (visit counts, radius) are repaired automatically
- The map for naming and confirming places is now zoomable and starts closer in; suggestions follow the visible map area
