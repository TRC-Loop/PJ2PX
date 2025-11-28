<p align="center">
  <img src="https://github.com/TRC-Loop/PJ2PX/blob/main/assets/PJ2PX.svg" width=50%/>
  <p align="center">Python · Jinja2 · PHP · HTML · CSS · JS</p>
</p>

---

# Python + Jinja2

## Site Generation
- Python: builds the site once
- Jinja2: templating engine for reusable templates and clean structure
- Poetry

## Frontend
- HTML: page structure and semantic markup
- CSS: styling, layout, and responsive design
- JavaScript: interactivity and client-side enhancements

## Backend
- PHP: used for some server-side includes or logic in the built pages
- SQLite3: lightweight database for storing content and configuration

## Features
- Static site: generated once, ready to deploy
- Modular and maintainable: clear separation between templates, frontend, and backend logic
- Lightweight stack: minimal dependencies, fast loading

# Real-world Examples

- [CronDNS](https://github.com/TRC-Loop/CronDNS)
- [GMRZE Website](https://gmrze.net)

> *Add your site to this list in a Pull Request*

# Folder Structure

This structure is recommended, but can be altered

```
.
├── build/
│   └── Files for build process
├── src/
│   ├── public/
│   │   ├── index.php
│   │   └── static/
│   │       ├── js
│   │       ├── css/
│   │       │   ├── styles.css
│   │       │   └── fonts.css
│   │       ├── images
│   │       └── fonts/
│   │           └── *.woff2
│   ├── templates/
│   │   ├── base.j2
│   │   └── *.j2
│   ├── macros/
│   │   └── *.j2
│   ├── conf/
│   │   └── config.php
│   └── lib/
│       └── *.php
├── config.yaml
├── build.py
├── pyproject.yml
└── README.md
```
> Made using [Tree](https://tree.nathanfriend.com/?s=(%27opti8s!(%27fancy5~fullPath!false~trailingSlash5~rootDot5)~B(%27B%2760Files%20for%206%20process3src0public7index97static7-j4H-styles.H-f8ts.Himage4f8t4-*.woff20templates7base.j2CmacrosCG7Gig90lib7*93Gig.yaml36.py3pyproject.yml3README.md3%27)~versi8!%271%27)-%20%2003-3%5Cn4s7-5!true6build70-8on9.phpBsource!C7*.j20Gc8fHcs4%01HGCB98765430-)

```
.
├── build/
│   └── Files for build process
├── src/
│   ├── public/
│   │   ├── all your webpages (*.php)
│   │   └── static/
│   │       ├── js/
│   │       │   └── all js files (*.js)
│   │       ├── css/
│   │       │   └── all css files, for large sites, make one css file per page (*.css)
│   │       ├── images/
│   │       │   └── all image files, try to only use webp and svg (*.webp, *.svg)
│   │       └── fonts/
│   │           └── holds all fonts (see fonts.css) mainly in woff2 or ttf format (*.ttf, *.woff2)
│   ├── templates/
│   │   └── holds all Jinja2 site templates (*.j2)
│   ├── macros/
│   │   └── holds all macros for you templates eg. navbar, footer, ... (*.j2)
│   ├── conf/
│   │   └── holds configuration files, like configuration for the database (*.php)
│   └── lib/
│       └── holds library files like an ORM or similar stuff as well as utilities (*.php)
├── config.yaml # Configuration file for your build process
├── build.py # Main entry-point for your build process
├── pyproject.yml # Auto-generated file by poetry (Python Configuration)
└── README.md
```
