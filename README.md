# nextReality.festival 2026 — Programm-App

Eine responsive Web-App für das Konferenzprogramm des [nextReality.festival 2026](https://nextrealityfestival.com/) in der Hamburger Speicherstadt.

## Features

- **Live-Indikator** — Zeigt die aktuell laufende Session an (basierend auf Echtzeit)
- **Favoriten** — Sessions mit Stern markieren, eigener Favoriten-Reiter (persistiert via localStorage)
- **Stage-Filter** — Zwischen Stages wischen (Mobile) oder per Pill-Navigation filtern
- **Kompakte Darstellung** — Session-Cards mit ausklappbaren Details
- **Responsive Layout** — Mobile (1 Spalte) → Tablet (2 Spalten) → Desktop (Multi-Column pro Stage)
- **Dark Mode** — Folgt System-Setting, mit manuellem Toggle (Auto / Hell / Dunkel)
- **Offizielles Logo** — Inline eingebettet, keine externen Abhängigkeiten

## Hosting auf GitHub Pages

1. Repository erstellen (z.B. `nextreality-festival-2026`)
2. `index.html` und `logo.png` in den Root pushen
3. **Settings → Pages → Source**: Branch `main`, Ordner `/ (root)`
4. Erreichbar unter `https://<username>.github.io/nextreality-festival-2026/`

> **Hinweis:** Das Logo ist als Base64 in der HTML-Datei eingebettet — die App funktioniert als einzelne Datei ohne externe Assets. `logo.png` ist die Full-Res-Version für andere Verwendungen.

## Programm anpassen

Die Session-Daten sind im `SESSIONS`-Array in `index.html` definiert. Festival-Datum: `FESTIVAL_DATES` und `DAY_LABELS` anpassen.

## Tech-Stack

- React 18 (CDN) · Vanilla CSS · Babel Standalone
- Zero Build — eine einzelne HTML-Datei, kein Build-Schritt nötig
- ~53 KB gesamt inkl. eingebettetem Logo

## Lizenz

Erstellt für nextReality.Hamburg e.V.
