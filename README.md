# Burgmann R-Bau – moderne statische Website

Statische Neuauflage der ehemaligen Webseite `www.burgmann.or.at`
(Burgmann R-BaugesmbH, Wiesen). Reines HTML/CSS/JS – kein Build-Schritt, keine
externen Abhängigkeiten, funktioniert komplett offline.

## Seiten

- `index.html` – One-Pager: Hero, Über uns, Leistungen (Planung/Ausführung/Koordination), Einblicke, Kontakt (mit `mailto:`-Formular)
- `musterhaeuser.html` – Musterhäuser (Haus I Pultdach/Satteldach, Haus II Pultdach/Single) mit Bildergalerien
- `referenzen.html` – Referenzen in 6 Kategorien mit Projektfotos
- `partner.html` – Partner-Links
- `impressum.html`, `datenschutz.html` – rechtliche Seiten (inkl. PDF-Download der Datenschutzerklärung)

## Struktur

```
├── index.html
├── musterhaeuser.html
├── referenzen.html
├── partner.html
├── impressum.html
├── datenschutz.html
└── assets/
    ├── css/style.css
    ├── js/main.js
    ├── img/            # Originalfotos/-logo (aus dem Web-Archiv der alten Seite)
    └── files/datenschutzerklaerung.pdf
```

## Lokal ansehen

```
python3 -m http.server 8000
# dann http://localhost:8000 aufrufen
```

## Deployment

Alle Dateien auf einen beliebigen statischen Hoster kopieren
(z. B. GitHub Pages, Netlify, Cloudflare Pages): `index.html` muss im
Wurzelverzeichnis liegen.

## Hinweise

- Inhalte und Bilder der alten Seite wurden aus der Wayback Machine
  (web.archive.org) rekonstruiert, da die Live-Seite automatisierte Zugriffe
  blockiert. Die Partner-Logos (logo1/4/6.jpg) waren nicht archiviert und sind
  daher als Text-Link-Karten umgesetzt.
- Das Kontaktformular nutzt `mailto:` und benötigt keinen Backend-Server.
