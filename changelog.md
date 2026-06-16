---
title: Changelog
description: What changed in each MapMyWay release.
---

# Changelog

## 1.2.11 — 2026-06-16


**Deutsch**

- „Alte Daten verdichten" arbeitet jetzt mit einem klaren Jahres-Stichtag: Du wählst „Vor JJJJ" statt „älter als X Jahre", damit immer eindeutig ist, was verdichtet wird.
- Neu: „Alte Daten löschen" — entfernt dauerhaft alle Einträge, Samples und danach unbenutzten Orte vor einem gewählten Jahr (mit zweistufiger Sicherheitsabfrage; die Aufzeichnung pausiert und läuft danach weiter).
- Neu: „Unbenutzte Orte löschen" — räumt Orte ohne verbleibende Besuche auf. Beide Lösch-Aktionen lassen die letzten Monate unangetastet.


**English**

- "Compact Old Data" now uses a clear yearly cutoff: pick "Before YYYY" instead of "older than X years", so it's always unambiguous what gets compacted.
- New: "Delete Old Data" — permanently removes all items, samples, and the places left unused from before a chosen year (two-step confirmation; recording pauses and resumes afterwards).
- New: "Delete Unused Places" — tidies up places with no visits left. Both delete actions leave the most recent months untouched.

## 1.2.10 — 2026-06-15


**Deutsch**

- Cloud- und Einstellungen-Tab aufgeräumt: Der iCloud-Status steht jetzt als eine ruhige Zeile (statt zwei großer Kacheln), der Einstellungen-Titel ist in der Serifenschrift der App, der Hilfe-Bereich ist eine Liste, und Texte wurden korrigiert (u. a. der irreführende Untertitel).
- Bedienungshilfen: Aufzeichnungs-Schalter sowie Einheiten- und Erscheinungsbild-Menüs haben jetzt VoiceOver-Beschriftungen.


**English**

- Tidied the Cloud and Settings tabs: iCloud status is now a single quiet line (instead of two large cards), the Settings title uses the app's serif, the Help area is a list, and some copy was corrected (including a misleading subtitle).
- Accessibility: the tracking toggle and the Units/Appearance menus now have VoiceOver labels.

## 1.2.9 — 2026-06-15


**Deutsch**

- Cloud-Tab aufgeräumt: Die Sicherungs-Aktionen stehen jetzt in logischer Reihenfolge — Jetzt sichern, wann zuletzt gesichert, Backups verwalten, Aus Backup wiederherstellen — und die Knöpfe haben einen einheitlichen Look.
- Im „Backups verwalten"-Dialog hat jeder Eintrag eigene Knöpfe für Wiederherstellen und Löschen (beide mit Sicherheitsabfrage).


**English**

- Tidied the Cloud tab: backup actions are now in a logical order — Backup Now, last-backup status, Manage Backups, Restore from Backup — with a uniform button look.
- In the "Manage Backups" dialog each entry now has its own Restore and Delete buttons (both with a confirmation prompt).

## 1.2.8 — 2026-06-15


**Deutsch**

- „Backups verwalten" aufgeräumt: Der Cloud-Tab zeigt nur noch einen Eintrag, der den Backup-Dialog öffnet. Im Dialog stehen jetzt voller Dateiname und Größe je Backup, der Speicherort (iCloud Drive › MapMyWay › Backups), und Löschen läuft über einen Papierkorb-Knopf statt Wischen (Antippen stellt wieder her).


**English**

- Tidied "Manage Backups": the Cloud tab now shows a single entry that opens the backup dialog. The dialog lists each backup's full filename and size, where they live (iCloud Drive › MapMyWay › Backups), and deletes via a trash button instead of swipe (tap a row to restore).

## 1.2.7 — 2026-06-14


**Deutsch**

- Neuer Bereich „Backups verwalten" (Cloud-Tab): zeigt deine iCloud-Backups mit echtem Datum, ein Tippen stellt ein Backup wieder her (mit Fortschrittsanzeige), und einzelne Backups lassen sich per Wischen löschen. Wiederherstellen ersetzt alle aktuellen Daten und wird vorher klar bestätigt.
- „Demo-Daten laden" fragt jetzt zweimal nach — damit Beispieldaten nicht versehentlich auf einem Gerät mit echten Aufzeichnungen geladen werden.


**English**

- New "Manage Backups" section (Cloud tab): shows your iCloud backups with their real date, tap one to restore it (with a progress readout), and swipe to delete individual backups. Restoring replaces all current data and is clearly confirmed first.
- "Load demo data" now asks twice — so sample data isn't loaded by accident on a device that already holds real recordings.

## 1.2.6 — 2026-06-14


**Deutsch**

- Behebt: Nach „Demo-Daten laden" gab es keinen sichtbaren Weg zurück zu den eigenen Daten — die App zeigte dann nur noch Beispieldaten. Der Demo-Bereich in den Einstellungen hat jetzt einen „Meine Daten anzeigen"-Schalter, der zurückschaltet und die Demo-Daten wieder entfernt. Deine echten Aufzeichnungen sind dabei nie betroffen — sie waren nur ausgeblendet, nicht gelöscht.


**English**

- Fix: after "Load demo data" there was no visible way back to your own data — the app would then show only sample data. The Demo section in Settings now has a "Show my data" action that switches back and removes the demo data. Your real recordings are never affected — they were only hidden, not deleted.

## 1.2.5 — 2026-06-14


**Deutsch**

- Akku im Hintergrund: Wenn iOS die App ohne Bildschirm aufweckt (für ein Standort-Ereignis), läuft jetzt nur noch die Aufzeichnung. Schwere Wartung — Aufräumen, Import-Reparatur, iCloud-Auflösung, Export-Nachholung — wartet, bis du die App öffnest. Spart Akku, besonders im Aufzeichnungsmodus ohne Status-Anzeige.
- Einstellungen → Batterie zeigt jetzt die App-Starts (Hintergrund- gegenüber Vordergrund-Starts) neben der CPU-Zeit — so siehst du, wie oft iOS die App im Hintergrund neu startet.


**English**

- Background battery: when iOS wakes the app without showing it (for a location event), only recording runs now. Heavy maintenance — cleanup, import repair, iCloud resolution, export catch-up — waits until you open the app. Saves battery, especially in the no-indicator recording mode.
- Settings → Battery now shows app launches (background vs foreground) next to CPU time, so you can see how often iOS relaunches the app in the background.

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
