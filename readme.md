# Entwicklerschuldenuhr

Was kostet ein Meeting? Die Seite rechnet aus den Stundensätzen der Teilnehmer aus, was eine bestimmte Dauer kostet, oder lässt die Kosten live mitlaufen. So wird verschwendete Zeit sichtbar.

Es ist eine einzelne HTML-Datei: nichts installieren, kein Server, keine Anmeldung.

## Benutzen

1. **`index.html` öffnen**: Doppelklick, die Seite läuft lokal im Browser.
2. **Personen-CSV anlegen** (siehe unten) und über "Datei auswählen" laden. Als Vorlage dient `beispiel.csv`.
3. **Teilnehmer ankreuzen**: nur wer im Meeting sitzt.
4. Dann eine der beiden Möglichkeiten:
   - **Feste Dauer**: Minuten eingeben oder per Schnellwahl (5/10/15/30/60) setzen, "Kosten anzeigen" drücken. Die Summe erscheint in einem eigenen Fenster.
   - **Live**: "Start (live)" drücken. Ein eigenes Fenster zeigt die laufenden Kosten (Update jede Sekunde) und die Zeit. "Stopp" friert den Stand ein. Erneutes Start setzt die Uhr zurück. Es gilt der Teilnehmerkreis beim Start.

Die Fenster lassen sich verschieben und in der Größe ändern, zum Beispiel auf den geteilten Bildschirm. Blockiert der Browser sie, einmalig Pop-ups für die Seite erlauben.

## Die CSV-Datei

Erste Zeile ist die Kopfzeile, danach eine Person pro Zeile:

```csv
Name;Stundensatz
Anna Beispiel;100
Ben Beispiel;100
Cem Beispiel;85,50
```

- Trennzeichen `;` oder `,` wird erkannt, Dezimalkomma ist erlaubt (`85,50`).
- Umlaute funktionieren, auch bei Excel-Export (UTF-8 oder Windows-1252).
- Fehlerhafte Zeilen meldet die Seite mit Zeilennummer, die übrigen Personen werden trotzdem geladen.
- Personen pflegst du ausschließlich in dieser Datei, die Seite ändert sie nicht.

## Datenschutz

- Die Stundensätze zeigt die Seite nie an. Die Ergebnisfenster enthalten nur die Summe, die Teilnehmerzahl und die Dauer.
- Nichts wird hochgeladen, alles läuft im Browser.
- Die zuletzt geladene CSV bleibt im Browser-Speicher (localStorage), damit du sie nicht jedes Mal neu wählen musst. Eine neu gewählte CSV ersetzt sie. Wer an deinem Rechner und Browser-Profil sitzt, kann die Daten dort einsehen. Es gibt keinen Passwortschutz.
- Die CSV selbst solltest du wie jede Gehaltsliste behandeln und nicht im Repo oder auf Freigaben ablegen. `beispiel.csv` enthält nur erfundene Werte.

## Begriffe

Siehe `GLOSSARY.md`.
