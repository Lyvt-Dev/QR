# QR

Kostenloser QR-Code-Generator ohne Wasserzeichen oder Registrierung. Inhalte und Logos werden lokal im Browser verarbeitet.

## Entwicklung

Voraussetzung: Node.js 20.19+ oder 22.12+ (getestet mit Node.js 24).

```sh
npm ci --cache /tmp/qr-npm-cache
npm run dev -- --port 5173
```

## Produktionsbuild

```sh
npm run build
npm run preview -- --port 4173
```

`dist/` kann auf einem statischen Webhost veröffentlicht werden. Es sind keine API-Schlüssel oder Backend-Dienste nötig. Google Fonts werden für die Darstellung geladen; bei fehlendem Zugriff verwendet die Seite Systemschriften.

## Funktionen

- Website, Text, E-Mail und WLAN
- Live-Vorschau, Farbpaletten, eigene Vordergrund- und Hintergrundfarben
- Punktformen, Ecken, Fehlerkorrektur, Ruhezone und eigenes Logo
- PNG, SVG, JPG und WebP, bis zu 4096 × 4096 Pixel
- Responsives Layout und Zurücksetzen aller Einstellungen

Die Codes sind statisch: Ihr Inhalt lässt sich nach dem Export nicht ändern. Farben und Logos können die Scanbarkeit beeinflussen; fertige Codes vor der Verwendung mit einem Scanner testen.
