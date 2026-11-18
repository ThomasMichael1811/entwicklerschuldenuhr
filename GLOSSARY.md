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

**Meeting-Ansicht**:
Die einzige Ansicht: CSV laden, Teilnehmer wählen, Dauer eingeben. Sie zeigt nur die Meetingkosten, nie einzelne Stundensätze. Die Personen werden ausschließlich manuell in der CSV gepflegt.
_Avoid_: Popup, Dashboard, Pflegeansicht
