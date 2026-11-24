# Burgmann R-Bau – moderne statische Website

Statische One-Pager-Neuauflage der ehemaligen Webseite `www.burgmann.or.at`
(Burgmann R-BaugesmbH, Wiesen). Reines HTML/CSS/JS – kein Build-Schritt, keine
Abhängigkeiten, funktioniert komplett offline.

## Struktur

```
burgmann-site/
├── index.html            # Startseite (Über uns, Leistungen, Region, Kontakt)
├── impressum.html        # Impressum
├── datenschutz.html      # Datenschutzerklärung
└── assets/
    ├── css/style.css     # modernes, responsives Design
    ├── js/main.js        # Mobile-Navigation, Scroll-Spy, Reveal-Animationen
    └── img/              # Platz für eigene Bilder/Logos
```

## Lokal ansehen

Variante 1 – direkt öffnen:

```
index.html im Browser öffnen
```

Variante 2 – lokaler Server (empfohlen, für korrekte Link-Auflösung):

```
cd burgmann-site
python3 -m http.server 8000
# dann http://localhost:8000 aufrufen
```

## Deployment

Alle Dateien auf einen beliebigen statischen Hoster kopieren
(z. B. Netlify, GitHub Pages, Cloudflare Pages, oder klassischer Webspace):
`index.html` muss im Wurzelverzeichnis liegen.

## Hinweise

- Die Bilder-Galerien der Originalseite (Musterhäuser, Referenzen, Partner-Logos)
  sind nicht enthalten, da die Originalbilder nicht mehr verfügbar waren.
  Eigene Bilder können in `assets/img/` abgelegt und in den HTML-Dateien
  verlinkt werden.
- Das Kontaktformular nutzt `mailto:` und benötigt keinen Backend-Server.
