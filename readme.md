# fortext lab webpage

Die Webseite läuft über GitHub Pages und basiert auf dem Theme/Template "Meme" von Hugo.

Alle möglichen Änderungen sollten in den Ordnern, die auf der gleichen Ebene wie diese README liegen, durchgeführt werden. Änderungen am Template sollten **nicht** im Ordner theme/meme durchgeführt werden.

# How to change content

## Inhaltliches

- Alle Inhalte/Unterseiten liegen unter `content/`. Im Content-Ordner gibt es einen Subordner für die englische und die deutsche Version der Webseite. Inhaltliche Anpassungen müssen entsprechend in beiden Ordnern umgesetzt werden.
- Die Subordner enthalten Markdown-Dateien, in denen letzlich die Inhalte der Unterseite stehen. Alle Unterseiten werden aktuell mit Hilfe von Shortcodes erstellt, die sich unter `layouts/shortcodes/` befinden. Folgende Unterseiten sind aktuell enthalten:
	- content/de/team.md : infos der Teammitglieder
	- content/de/_index.md : Startseite
	- content/de/projekte.md: Alle Projekte
	- content/de/pubs.md: Ruft einen Shortcode auf, der unter `layouts/` liegt und die Publikationsliste als HTML-Datei enthält. Die Publikationsliste wird wiederum mit einem Notebook generiert, das [im Codesnippets-Repo](https://github.com/forTEXT/Codesnippets/blob/main/Webseiten/labpublications.ipynb) liegt.

	- Alte Ordner: projects_deprected, projects_old, team_old

## Bilder

- Alle Webseitenbilder und Logos befinden sich unter `static/images/`:	
	- lab_team : Fotos der Teammitgliedern
	- overview : Sammlung von Labübersichtsversionen auf der Landing Page
	
## Themeeinstellungen (Navigation, Sprache)

- Alle möglichen "Grundeinstellungen" müssen in der `config.toml`-Datei getroffen werden. Besonders relevant sind hier.
- Änderungen am Layout etc. sollten in den Ordnern auf der gleichen Ebene wie diese README durchgeführt werden, nicht aber im Originaltemplate, das sich unter `themes/meme` befindet.

# Directory Structure

.
├── README.md
├── archetypes
│   └── default.md
├── assets
│   └── scss
├── config.toml
├── content --> Für inhaltliche Anpassungen nutzen
│   ├── de
│   │   ├── _index.md
│   │   ├── projects_deprecated
│   │   │   ├── Diss_publikationsreihen.md
│   │   │   ├── Forschungsprojekte.md
│   │   │   └── Software.md
│   │   ├── projects_old
│   │   │   ├── Research
│   │   │   │   ├── _index.md
│   │   │   │   ├── d-prose.md
│   │   │   │   ├── event.md
│   │   │   │   ├── katkit.md
│   │   │   │   ├── konflikte.md
│   │   │   │   ├── plans.md
│   │   │   │   └── szenen.md
│   │   │   ├── Software
│   │   │   │   ├── _index.md
│   │   │   │   ├── catma.md
│   │   │   │   ├── catma.png
│   │   │   │   └── gitma.md
│   │   │   └── dis_pub_reihen
│   │   │       ├── _index.md
│   │   │       ├── fortext.md
│   │   │       ├── fortext_hefte.md
│   │   │       └── jcls.md
│   │   ├── projekte.md
│   │   ├── pubs.md
│   │   ├── team.md
│   │   └── team_old
│   │       ├── _index.md
│   │       ├── a_gius
│   │       │   └── bio.md
│   │       ├── akazawa
│   │       │   └── bio.md
│   │       ├── gerstorfer
│   │       │   └── bio.md
│   │       ├── guhr
│   │       │   └── bio.md
│   │       ├── haeussler
│   │       │   ├── bio.md
│   │       │   └── haeussler.png
│   │       ├── meister
│   │       │   ├── bio.md
│   │       │   └── meister.png
│   │       └── stiemer
│   │           ├── bio.md
│   │           └── stiemer.png
│   └── en
│       ├── _index.md
│       ├── projects_deprecated
│       │   ├── Diss_publikationsreihen.md
│       │   ├── Research.md
│       │   └── Software.md
│       ├── projekte.md
│       ├── pubs.md
│       └── team.md
├── data
│   ├── SVG.toml
│   └── Socials.toml
├── layouts --> HTML-Seiten etc. unter shortcodes ergänzen
│   ├── _default
│   ├── partials
│   └── shortcodes
├── public --> Automatisch generierter Ordner
├── requirements.txt
├── resources
├── static --> enthält Bilder
├── themes

113 directories, 267 files
