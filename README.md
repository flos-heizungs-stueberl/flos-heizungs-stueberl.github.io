# Flos Heizungsstüberl — GitHub Pages Website

Kurze Anleitung und Hinweise zum Projekt (erste Entwurfs‑Website).

## Was ist hier
- Statische Website für Flos Heizungsstüberl (GitHub Pages).
- Enthaltene Seiten: `index.html`, `speisekarte.html`, `veranstaltungen.html`, `stammtisch.html`, `hochzeiten.html`, `kontakt.html`, `gallery.html`, `impressum.html`.
- Styling: `styles.css`.
- Platz für Logos / Bilder: `Logos/` (lege hier `untersberg.jpg`, `hofbrauhaus_berchtesgaden.jpg`, `franziskaner.jpg`, `hargassner.jpg`, `Laura_Berg.jpg` ab).

## Schnellstart lokal (PowerShell)
1. Im Projektordner prüfen:
   ```powershell
   cd 'c:\Users\s1u21oc\OneDrive - Volkswagen AG\Dokumente\10_Projekte\2026_homepage_test\flos-heizungs-stueberl.github.io'
   ```
2. Änderungen committen (wenn noch nicht gemacht):
   ```bash
   git add -A
   git commit -m "Update site"
   ```
3. Push (bereits eingerichtet):
   ```bash
   git push
   ```

## Temporären Commit‑Author nur für einen Commit setzen
- Einmalig beim Commit (ändert nicht die globalen Einstellungen):
  ```bash
  git commit --author="flos-heizungs-stueberl <ponnei@gmx.de>" -m "Commit message"
  ```
- Oder temporär für einen Befehl:
  ```bash
  git -c user.name="flos-heizungs-stueberl" -c user.email="ponnei@gmx.de" commit -m "Commit message"
  ```

## GitHub Pages aktivieren
- Repository → Settings → Pages (oder Code and automation → Pages): Source = Branch `main`, Folder = `/ (root)` auswählen.
- Bei `username.github.io` wird die Seite unter `https://username.github.io/` veröffentlicht.

## Eigene Domain (optional, kostenlos aber DNS‑Änderungen nötig)
- Datei `CNAME` im Repo mit der Domain (z. B. `www.deinedomain.de`) anlegen.
- DNS: Setze A‑Records auf GitHub IPs oder CNAME auf `username.github.io` (siehe GitHub Pages‑Doku).

## Formulare & WhatsApp
- Kontakt- / Event-Formulare nutzen FormSubmit (FormSubmit leitet Mails an `ponnei@gmx.de`).
- Für direkte WhatsApp‑Anfragen ist ein Button integriert (`kontakt.html`) mit Link `https://wa.me/491718906893?text=...` — öffnet WhatsApp am Gerät.
- Für automatisches WhatsApp (Empfang von Formularen) brauchst du Dienste wie Twilio + Zapier/Make (kostenpflichtig & DSGVO‑Pflichten beachten).

## Bilder & Logos
- Lege die endgültigen Logos/Bilder in `Logos/` ab. Benutze gleiche Dateinamen wie in HTML (z. B. `hofbrauhaus_berchtesgaden.jpg`).
- Bilder sollten lizenzfrei oder von dir freigegeben sein (achtung Markenlogos).

## Google Maps / Google Business
- Um in Google Maps als Unternehmen zu erscheinen: Erstelle ein Google Business Profile (kostenlos), bestätige Adresse/Telefon (Postkarte oder Telefon) und fülle Öffnungszeiten/Infos aus.

## Rechtliches (Deutschland)
- Impressum & Datenschutzerklärung sind erforderlich. Prüfe die Angaben in `impressum.html` und ergänze ggf. USt‑ID, Betreiberdaten, Verantwortlichen.

## Weiteres / Tipps
- Mobile testen: Cache leeren, ggf. `?v=1` an CSS hängen beim Entwickeln (z. B. `styles.css?v=2`) um Browsercache zu umgehen.
- SEO: Metatags & OpenGraph ergänzen (optional).
- Wenn du willst, erstelle ich ein README‑Release, eine Sitemap oder helfe bei DNS/Domain‑Einrichtung.

## Kontakt
- Bei Fragen zur Implementierung oder wenn du Bilder/Logos hochlädst, sag mir Bescheid — ich übernehme die Integration.

---

Kurzer Entwicklungsstand: erste Version live gepusht (Branch `main`).

