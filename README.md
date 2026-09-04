# Jorge Cortez - CV Website

A modern, responsive CV/resume website built with Eleventy (11ty) and Tailwind CSS.

## Description

This is a personal CV website for Jorge Cortez, a Senior Full Stack Developer, Lead Mobile UI/UX Developer, and User Centered Design specialist. The site showcases professional experience, education, skills, and projects.

## Tech Stack

- **Eleventy (11ty)** - Static site generator
- **Tailwind CSS** - Utility-first CSS framework
- **Nunjucks** - Templating engine
- **PostCSS & Autoprefixer** - CSS processing
- **npm-run-all** - Script management

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ElBatou/jorge-cortez-cv.git
cd jorge-cortez-cv
```

2. Install dependencies:
```bash
npm install
```

## Development

Run the development server with hot-reload:
```bash
npm start
```

This will:
- Start Eleventy in serve mode (available at `http://localhost:8080`)
- Watch and compile Tailwind CSS
- Auto-reload on file changes

## Build

Build the site for production:
```bash
npm run build
```

The built files will be output to the `_site` directory.

## Project Structure

```
jorge-cortez-cv/
├── src/
│   ├── assets/
│   │   ├── css/
│   │   │   └── tailwind.css       # Main Tailwind CSS entry point
│   │   └── images/                # Static images (logos, icons, etc.)
│   ├── _data/
│   │   └── site.json              # Site metadata
│   ├── _includes/
│   │   ├── partials/
│   │   │   ├── _header.njk        # Header component
│   │   │   └── _footer.njk        # Footer component
│   │   ├── sections/
│   │   │   ├── experience.njk     # Experience section
│   │   │   ├── education.njk      # Education section
│   │   │   ├── skills.njk         # Skills section
│   │   │   └── projects.njk       # Projects section
│   │   └── shortcodes/
│   │       └── pageHeading.js     # Custom Nunjucks shortcode
│   ├── _layouts/
│   │   └── base.njk               # Base layout template
│   └── index.njk                  # Homepage
├── _site/                         # Build output (generated)
├── eleventy.config.js              # Eleventy configuration
├── tailwind.config.js              # Tailwind CSS configuration
├── postcss.config.js               # PostCSS configuration
└── package.json                    # Project dependencies and scripts
```

## Configuration

### Eleventy
- **Input directory**: `src/`
- **Output directory**: `_site/`
- **Path prefix**: `/jorge-cortez-cv/` (for GitHub Pages deployment)
- **Template engine**: Nunjucks

### Tailwind CSS
- **Content paths**: `./src/**/*.{njk,md,js}` and `./src/**/*.svg`
- **Custom animations**: Includes a custom shake animation for icons

## Custom Shortcodes

The site includes custom Nunjucks shortcodes:
- `pageHeading` - Renders section headings
- `currentYear` - Returns the current year

## Deployment

The site is configured for GitHub Pages deployment with the path prefix `/jorge-cortez-cv/`. To deploy:

1. Push changes to the repository
2. Configure GitHub Pages to serve from the `_site` directory
3. Set the build command to `npm run build`

## License

ISC

## Author

Jorge Cortez - [GitHub](https://github.com/ElBatou)
