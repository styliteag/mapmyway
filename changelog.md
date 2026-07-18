---
title: Changelog
description: What changed in each MapMyWay release.
---

# Changelog

## 1.2.21 — 2026-07-18


**Deutsch**

- Lange „ewige“ Fahrten, die nicht enden, werden verhindert: Stops werden wieder als Besuch erkannt.
- Die Aufzeichnung im Hintergrund bleibt länger aktiv, bis der Sleep-Modus greift.
- Orphaned GPS-Samples werden nicht mehr fälschlich an eine laufende Fahrt gehängt.


**English**

- Prevents long “eternal” trips that never end: stops are recognized as visits again.
- Background recording stays active until sleep mode can take over.
- Orphaned GPS samples are no longer wrongly attached to an ongoing trip.

## 1.2.20 — 2026-07-17


**Deutsch**

- Fahrten werden nach einem Neustart zuverlässiger weiterverarbeitet, damit keine langen, leeren Fahrten entstehen.
- Die Aufzeichnung im Hintergrund ist stabiler.


**English**

- Trips are processed more reliably after restarting the app, preventing long empty trips.
- Background recording is more reliable.

## 1.2.19 — 2026-07-15


**Deutsch**

- Deutlich weniger Schreiblast auf der Datenbank: Jeder aufgezeichnete Punkt wird jetzt nur noch einmal gespeichert statt zweimal. Das senkt den Stromverbrauch im Hintergrund weiter und schont den Speicher.
- Zweite Absicherung gegen Aufzeichnungslücken: Die Aufnahme-Engine hält sich nach einem Neustart durch iOS jetzt auch selbst am Leben, bis die Aufzeichnung verankert ist — zusätzlich zum Schutz aus 1.2.18.


**English**

- Much lower database write load: every recorded point is now saved once instead of twice. This further reduces background battery drain and eases storage wear.
- Second safeguard against recording gaps: the recording engine now also keeps itself alive after an iOS relaunch until recording is anchored — on top of the protection added in 1.2.18.

## 1.2.18 — 2026-07-15


**Deutsch**

- Zuverlässigere Aufzeichnung im Hintergrund: Wenn iOS die App nach einer Pause neu startet, hält sie sich jetzt selbst am Leben, bis die Aufzeichnung wieder stabil läuft. Vorher konnten dabei stundenlange Lücken in der Timeline entstehen und besuchte Orte wurden nicht erkannt.
- Die Genauigkeits-Einstellung (Hoch/Mittel/Niedrig) ist entfernt. Die App nutzt jetzt immer das stromsparende GPS-Tuning der Aufnahme-Engine — gleiche Ortserkennung, deutlich weniger Akkuverbrauch, besonders über Nacht.


**English**

- More reliable background recording: when iOS relaunches the app after a pause, it now keeps itself alive until recording is fully anchored again. Previously this could leave hours-long gaps in your timeline and visited places went undetected.
- The accuracy setting (High/Balanced/Low) has been removed. The app now always uses the recording engine's power-efficient GPS tuning — same place detection, noticeably less battery drain, especially overnight.

## 1.2.17 — 2026-07-11


**Deutsch**

- Kein Standort-Pfeil mehr: Die Aufzeichnung läuft jetzt über einen neuen Hintergrund-Mechanismus, der ohne den Pfeil in der Statusleiste auskommt — und trotzdem lückenlos aufzeichnet.
- Die Auswahl „Hintergrund-Aufzeichnung" (Pfeil / Kein Pfeil / Sparmodus) entfällt: Der neue Mechanismus vereint alle drei Vorteile (lückenlos, kein Pfeil, sparsam), ein Kompromiss ist nicht mehr nötig. Die Genauigkeits-Einstellung bleibt.
- Abfahrten nach längeren Stopps sollten deutlich schneller erkannt werden als bisher im Sparmodus.
- Bitte testen: Wird eine Fahrt direkt nach einem langen Halt sofort erfasst? Bleibt die Statusleiste wirklich frei vom Pfeil? Und wie entwickelt sich die Batterie über 1–2 Tage — auch nach dem manuellen Beenden der App?


**English**

- No more location arrow: recording now uses a new background mechanism that works without the status-bar arrow — while still recording without gaps.
- The "Background Recording" choice (Arrow / No arrow / Saver) is gone: the new mechanism combines all three benefits (gapless, no arrow, frugal), so there is no trade-off to pick anymore. The Accuracy setting stays.
- Departures after longer stops should be detected much faster than in the previous battery-saver mode.
- Please test: does a trip right after a long stop get captured immediately? Does the status bar really stay free of the arrow? And how does battery hold up over 1–2 days — including after force-quitting the app?

## 1.2.16 — 2026-07-02


**Deutsch**

- Deutlich sparsamer beim Akku: halb so viele Datenbank-Schreibzyklen während der Aufzeichnung, sparsamere Verarbeitung der Ortungsdaten bei Autofahrten, und die App verzichtet im Hintergrund auf unnötige Anzeige-Aktualisierungen und Statusabfragen.
- Automatische Exporte laufen nur noch, wenn das Gerät lädt, und werden nach längeren Pausen in Etappen nachgeholt statt in einem großen Schub.
- Aktivitätserkennung im Hintergrund läuft jetzt garantiert ohne Grafikchip — stabiler und stromsparender.
- Korrigierte Modus-Beschreibung: Am wenigsten Akku braucht „Battery saver", nicht der Modus mit Standort-Pfeil.
- Bitte testen: Batterielaufzeit über 1–2 Tage normaler Nutzung beobachten und Auffälligkeiten melden.


**English**

- Much easier on the battery: half the database write cycles while recording, leaner location processing during drives, and no more unnecessary display refreshes or status polling while the app is in the background.
- Automatic exports now only run while the device is charging, and catch up in stages after longer gaps instead of one big burst.
- Background activity recognition now runs guaranteed GPU-free — more stable and more power-efficient.
- Corrected mode description: "Battery saver" uses the least battery, not the mode with the location arrow.
- Please test: watch battery life over 1–2 days of normal use and report anything unusual.

## 1.2.12 — 2026-06-16


**Deutsch**

- „Unbenutzte Orte löschen" und „Alle Daten löschen" zeigen jetzt sofort einen Ladekreis, während im Hintergrund gezählt wird — vorher wirkte der Knopf ein paar Sekunden lang tot, bis die Abfrage erschien.


**English**

- "Delete Unused Places" and "Wipe All Data" now show a spinner the moment you tap, while the counts are gathered in the background — previously the button looked dead for a few seconds until the prompt appeared.

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
