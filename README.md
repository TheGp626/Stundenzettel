# Stundenzettel PWA

digitaler Stundennachweis für Lübbert Event Interiors. gebaut weil ich keine Lust mehr hatte papier rumzuschleppen.

läuft als PWA, also installierbar auf android, funktioniert offline, sieht aus wie eine app.

## was es kann

- woche auswählen, tage aufklappen, zeiten eintragen
- mehrere schichten pro tag (z.b. auf- und abbau am selben tag)
- pause wird automatisch berechnet (0 / 30 / 45 min je nach stunden)
- minimum 3h pro schicht wird automatisch angerechnet
- AL name + unterschrift direkt im feld zeichnen
- als PDF exportieren
- wochen lokal speichern und wieder laden
- dark/light/auto theme

## benutzen

1. name rein, woche auswählen
2. tag aufklappen
3. von/bis eintragen, ort wenn nötig
4. AL unterschreiben lassen
5. speichern oder direkt als PDF raus

## lokal testen

```bash
python -m http.server 4173
```

dann `http://localhost:4173` im browser

## deployment

einfach die 4 dateien/ordner auf github pages schmeißen:

```
index.html
sw.js
manifest.json
icons/
```

settings → pages → branch main / root → save. fertig.
