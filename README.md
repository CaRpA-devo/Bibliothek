# CodeConnect – Entwickler-Bibliothek

## Überblick

CodeConnect bündelt kuratierte Ressourcen für Webentwickler:innen an einem Ort. Die Anwendung ist als statische Website ausgelegt und liefert Links zu Lernplattformen, Dokumentationen, Design-Tools sowie einer umfangreichen Video-Sammlung. Ziel ist es, Einsteiger:innen wie Fortgeschrittenen einen schnellen Zugriff auf nützliche Quellen für Frontend-, Backend- und Fullstack-Entwicklung zu ermöglichen.

## Kernfunktionen

- **Zentrale Link-Sammlung**: Kategorien für Fonts, Farben, Bilder, Frameworks, Tools, Generatoren, Animationen, Icons, Self-Learning und Dokumentationen.
- **CourseWiki-Übersicht**: Kartenansicht mit direkten Verweisen auf Lernmaterial von CourseWiki (UI/UX, Layout, Daten, Animationen, Grid, Flexbox u.v.m.).
- **Video-Karussell**: Mit Swiper.js realisierte Slider-Komponente für YouTube-Tutorials zu gängigen Web-Technologien.
- **Kontaktbereich**: Kontaktinformationen und Formular, das über Formspree ansprechbar ist.
- **Responsives Layout**: Moderne Gestaltung mit CSS Grid, Flexbox und individuellen Komponenten.

## Projektstruktur

```text
.
├── codeconnect.html        # Haupteinstiegspunkt der Anwendung
├── codeconnect.css         # Zentrales Styling (Layout, Bento-Grid, Slider, Komponenten)
├── swiper.js               # Initialisierung und Konfiguration des Sliders
├── src/
│   ├── fonts/              # Lokale Schriftarten (Roboto Condensed, Work Sans)
│   └── pictures/           # Assets für Bento-Bilder, Logos, Hintergrundgrafiken
├── LICENSE                 # MIT-Lizenz
└── README.md               # Dieses Dokument
```

## Schnellstart

1. Projekt klonen oder herunterladen:
   ```bash
   git clone https://github.com/CaRpA-devo/Bibliothek.git
   ```
2. Verzeichnis öffnen und `codeconnect.html` im Browser laden.
3. Optional einen lokalen Webserver starten (z. B. mit VS Code Live Server), um relative Pfade und Formspree-Formulare ohne Einschränkungen zu testen.

## Entwicklung & Anpassung

- **Layout & Styling**: Anpassungen erfolgen in `codeconnect.css`. Dort sind u. a. Bento-Grid, Navigationsleiste, Slider, Karten und Formular-Styles definiert.
- **Inhalte pflegen**: Linklisten und Texte liegen direkt in `codeconnect.html`. Neue Ressourcen können durch Ergänzen der Listen-Elemente (`<li>`) hinzugefügt werden.
- **Swiper-Konfiguration**: Einstellungen wie Loop, Slides pro View oder Pagination befinden sich in `swiper.js`. Weitere Optionen sind in der [Swiper-Dokumentation](https://swiperjs.com/swiper-api) beschrieben.
- **Assets**: Eigene Bilder oder Videos werden unter `src/pictures/` abgelegt; Fonts unter `src/fonts/`. Achte auf konsistente Pfade innerhalb der HTML-Datei.
- **Formular**: Das Kontaktformular sendet über Formspree (`https://formspree.io/f/mzzdrbvo`). Für andere Empfänger einfach die Action-URL tauschen.

## Technologien & Abhängigkeiten

- Statische HTML5-Struktur (`codeconnect.html`)
- Individualisiertes CSS (ohne Präprozessor)
- [Font Awesome](https://fontawesome.com/) via CDN
- [Swiper.js](https://swiperjs.com/) via CDN für das Tutorials-Karussell
- Lokale Webfonts (Roboto Condensed, Work Sans)
- Formspree für Formular-Handling

## Deployment-Hinweise

- Projekt kann als statische Seite auf jedem Hosting-Dienst (GitHub Pages, Netlify, Vercel, etc.) betrieben werden.
- Stelle sicher, dass alle Assets aus `src/pictures/` und `src/fonts/` mitdeployt werden.
- Für optimale Ladezeiten bietet sich an, Bilder vorab zu komprimieren.

## Lizenz

Dieses Projekt steht unter der [MIT-Lizenz](./LICENSE). Bitte beachte bei externen Ressourcen (YouTube-Videos, Drittanbieter-Links) die jeweiligen Nutzungsbedingungen.
