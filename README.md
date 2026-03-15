# Flos Heizungsstüberl — GitHub Pages Website

Kurzbeschreibung und aktueller Stand der statischen Website.

## Inhalt des Repos
- Statische Website für Flos Heizungsstüberl (für GitHub Pages).
- Enthaltene Seiten: `index.html`, `speisekarte.html`, `veranstaltungen.html`, `stammtisch.html`, `hochzeiten.html`, `kontakt.html`, `gallery.html`, `ueber-uns.html`, `impressum.html`.
- Styling: `styles.css`.
- Medienordner: `Bilder/`, `Logos/`, `Videos/` (lokale Bilder und Videos sind bereits eingebunden).

## Aktueller Stand
- Design: modernes, responsives Layout mit einheitlichem Header auf allen Seiten.
- Inhalte: alle Hauptseiten sind erstellt und lokal angepasst (Navigation, Galerie, Veranstaltungen, Über‑uns‑Seite, Kontaktformular, Hochzeitsanfrage).
- Mobile: mehrere Optimierungen vorgenommen (siehe Abschnitt "Mobile Optimierungen").
- Hinweis: Alle Änderungen wurden lokal umgesetzt. Es erfolgt erst ein Commit & Push, wenn du explizit zustimmst.

## Schnellstart lokal
1. Öffne ein Terminal und wechsel in das Projektverzeichnis (Projekt-Root).
2. Vorschau:
   - Einfach: Datei `index.html` im Browser öffnen.
   - Alternativ (lokaler HTTP‑Server):
     - Python: `python -m http.server 8000` und dann im Browser `http://localhost:8000` öffnen.
     - Oder benutze eine Live‑Server-Erweiterung in deinem Editor.
3. Git‑Workflow (Beispiele):
   ```bash
   git add -A
   git commit -m "Update site"
   git push origin main
   ```
   (Die finale Commit/Pull/Push‑Aktion wird erst nach deiner Freigabe ausgeführt.)

## Formulare & Kontaktlinks
- Die auf der Seiten verwendeten Formulare senden an die in den Formular-Elementen hinterlegten Ziele. Prüfe bei Bedarf die `action`‑Attribute in den jeweiligen HTML‑Dateien.
- Der WhatsApp‑Link ist als Platzhalter in `kontakt.html` hinterlegt; passe die Zielnummer dort an, falls nötig.

## Bilder & Logos
- Lege endgültige Logos/Bilder in `Logos/` bzw. in `Bilder/` ab. Verwende die in den HTML‑Dateien referenzierten Dateinamen.
- Empfehlung: Für bessere Ladezeiten Mobile‑optimierte Versionen (WebP/JPEG in kleinerer Auflösung) und `srcset` verwenden.

## Mobile Optimierungen — durchgeführt
- Hintergrund: auf mobilen Geräten wird `background-attachment: scroll` verwendet, Overlay‑Opacity reduziert für bessere Lesbarkeit.
- Hero: responsive (Bild skaliert, Textgröße angepasst für kleine Displays).
- Navigation: Hamburger‑Pattern für kleine Bildschirme (nav versteckt/ausklappbar).
- Bilder: Lazy‑Loading eingesetzt, Lazy‑Helper so angepasst, dass Bilder nicht unsichtbar bleiben, falls JS nicht greift.

## Mobile Optimierungen — Empfehlungen
- Bildformate: Erzeuge mobile WebP/AVIF Varianten und nutze `srcset`/`sizes` für schnellere Ladezeiten.
- Kritische CSS: Falls weitere Performance nötig ist, extrahiere kritische CSS für den First Paint.
- Script‑Defer: Nicht-kritische Skripte `defer` oder ans Ende setzen.
- Test: Auf langsamen Mobilfunkverbindungen testen (Throttling, Lighthouse) und ggf. Hero‑Bild weiter verkleinern.

## Rechtliches / Hinweise
- Prüfe Impressum & Datenschutzerklärung auf Vollständigkeit und Richtigkeit.
- Achte bei Verwendung von Markenlogos auf rechtliche Nutzungsbedingungen.

Wenn du möchtest, übernehme ich das Committen & Pushen mit einem temporären Author‑Attribut — antworte dazu mit „Freigabe“. Wenn du noch Inhalte oder weitere Mobile‑Anpassungen willst, nenne bitte die gewünschten Änderungen kurz.

