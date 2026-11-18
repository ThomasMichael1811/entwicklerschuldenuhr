# Entwicklerschuldenuhr

Eine Seite, die zeigt, was ein Meeting an Personalkosten verursacht, damit verschwendete Zeit sichtbar wird.

## Language

**Person**:
Ein Eintrag in der CSV-Datei mit Name und Stundensatz.
_Avoid_: Mitarbeiter, Entwickler, Kollege

**Teilnehmer**:
Eine Person, die für ein bestimmtes Meeting ausgewählt ist.
_Avoid_: Person (wenn das konkrete Meeting gemeint ist)

**Stundensatz**:
Die Kosten einer Person pro Stunde in Euro.
_Avoid_: Gehalt, Tagessatz

**Meetingkosten**:
Die Summe aus Stundensatz mal Dauer über alle Teilnehmer.
_Avoid_: Gesamtkosten, Schulden

**Pflegeansicht**:
Die Ansicht zum Importieren und Prüfen der Personen mit ihren Stundensätzen, nur für den Besitzer gedacht.
_Avoid_: Admin, Einstellungen

**Meeting-Ansicht**:
Die Ansicht, die im Meeting sichtbar ist und nur die Meetingkosten zeigt, nie einzelne Stundensätze.
_Avoid_: Popup, Dashboard
