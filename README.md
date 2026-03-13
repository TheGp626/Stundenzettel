# Stundenzettel (PWA)

Einfache Web‑App zum Erfassen von Arbeitszeiten pro Kalenderwoche, inklusive:

- mehreren Schichten pro Tag
- automatischer Pausenberechnung
- Ort / Venue pro Tag
- AL‑Unterschrift (Fullscreen-Signaturpad)
- PDF‑Export
- Offline/PWA Unterstützung (Service Worker)

## Nutzung

1. Name und Kalenderwoche eintragen.
2. Tage aufklappen und Schichten eintragen (`Von` / `Bis`).
3. Optional: Ort / Venue und Name AL erfassen.
4. Für Signatur:
   - auf das Signaturfeld tippen **oder**
   - auf den Button `Vollbild` im Signaturfeld drücken.
5. Mit `Woche speichern` lokal speichern.
6. Mit `Als PDF exportieren` Nachweis exportieren.

## Signatur-Hinweis (wichtig)

Wenn Signatur auf einem Gerät nicht öffnet:

- zuerst den `Vollbild`-Button im Signaturfeld nutzen (harter Fallback),
- dann Browser/PWA einmal neu laden,
- bei installierter App ggf. App schließen und neu öffnen.

Die App versucht Fullscreen + Landscape bei Signatur automatisch (wenn vom Browser erlaubt).

## Lokal starten

```bash
python -m http.server 4173
```

Dann im Browser öffnen: `http://localhost:4173`

## Deployment

Statische Dateien:

- `index.html`
- `sw.js`
- `manifest.json`
- `icons/*`

Für GitHub Pages direkt geeignet.
