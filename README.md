# Jaguar

A static clone of the Jaguar India homepage, built with plain HTML and CSS as a front-end practice project. It is a personal learning project and is not affiliated with Jaguar Land Rover.

Live site: https://codewith-vivek.github.io/Jaguar/

## Features

The page is a single `index.html`, built section by section. Each section has its own stylesheet.

| Section | What it shows | Stylesheet |
| --- | --- | --- |
| Header | Logo plus Vehicles, Purchase, Owners, Explore, Retailers and Builds links | `header.css` |
| Hero | Muted video that autoplays and loops, with menu and pause icons | `section-2.css` |
| Models | Jaguar F-PACE and I-PACE cards with prices and "Design yours" / "Explore" actions | `section-3.css` |
| Racing banner | Jaguar TCS Racing image with slide dots, arrows and a "learn more" link | `section-4.css` |
| Quick actions | Four "Book a test drive" tiles with icons | `section-5.css` |
| Link directory | Footer link columns and social icons (Facebook, X, YouTube, Instagram, LinkedIn) that swap to a second image on hover | `section-6.css` |
| Search | Site search input | `section-7.css` |
| Legal | Market, careers, terms and privacy links, then the legal footer text | `section-8.css` |

`general.css` holds the shared base styles.

### Current limitations

- There is no JavaScript. The carousel dots and arrows, the pause button and the search box are visual only.
- Most links are `<a>` tags with no `href`, so they are placeholders.
- There are no `@media` queries, so the layout is designed for desktop widths only.
- The CSS names `ProximaNova` and `AvenirNext`, but no font files are loaded. Browsers fall back to Arial or Helvetica unless those fonts are installed.

## Tech stack

- HTML5
- CSS3

There is no framework, build tool, package manager or JavaScript.

## Folder structure

```
.
├── index.html              # Entry page (the only page)
├── assets/
│   ├── css/                # general.css, header.css, section-2.css … section-8.css
│   ├── icons/              # UI icons and favicon.png
│   │   └── social/         # Social icons: <name>.png and <name>-hover.png
│   ├── images/
│   │   ├── cars/           # Model images (car-1.png, car-2.png)
│   │   ├── logo/           # jaguar-logo.png
│   │   ├── luxury.png      # Racing banner image
│   │   └── jaguar-1.avif   # Not referenced by index.html yet
│   └── videos/             # jaguar-after-hours.mp4 (hero video)
├── .editorconfig           # Editor settings (UTF-8, LF, 4-space indent)
├── .gitignore
└── README.md
```

## Prerequisites

- A modern web browser.
- Optional: any static file server, if you prefer serving over opening the file directly.

## Setup

```
git clone https://github.com/CodeWith-vivek/Jaguar.git
cd Jaguar
```

Nothing needs to be installed.

## Environment variables

None. The project does not read any configuration or environment variables.

## Development

There are no dev scripts. Open `index.html` in a browser and reload after editing.

Conventions:

- File and folder names use lowercase kebab-case.
- Asset paths are relative to `index.html`.
- Each page section has its own stylesheet in `assets/css/`.

## Build and run

There is no build step. The files in the repository are served as they are. To run the site, open `index.html` or serve the repository root with any static server.

## Tests

There are no tests.

## Deployment

The site is served by GitHub Pages from this repository at https://codewith-vivek.github.io/Jaguar/. There is no CI workflow in the repo. Pages publishes the branch as it is, so pushing to the Pages source branch updates the live site.
