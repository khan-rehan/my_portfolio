# My Portfolio v2

A personal developer portfolio website built with Gatsby and React, featuring a blog (Pensieve), project showcase, work experience timeline, and a modern dark-themed design.

**Live Site:** [rehankhan.tech](https://rehankhan.tech/)
**Previous Version:** [v1](https://rehankhan.netlify.app/)

## Features

- Single-page portfolio with smooth scrolling navigation
- Hero, About, Work Experience, Featured Projects, Projects, and Contact sections
- Blog section (Pensieve) with Markdown-based posts, tagging, and syntax highlighting
- Responsive design for mobile and desktop
- Scroll-triggered animations using ScrollReveal and Anime.js
- SEO optimized with sitemap, robots.txt, and Open Graph meta tags
- PWA support with offline capability
- Google Analytics integration
- Markdown-driven content — all projects, jobs, and posts are stored as `.md` files

## Tech Stack

- **Framework:** Gatsby v4, React v17
- **Styling:** Styled Components
- **Content:** Markdown + GraphQL
- **Animations:** Anime.js, ScrollReveal, React Transition Group
- **Code Highlighting:** Prism.js
- **SEO:** React Helmet, gatsby-plugin-sitemap, gatsby-plugin-robots-txt
- **Deployment:** Netlify / GitHub Pages

## Project Structure

```
my_portfolio/
├── content/               # Markdown content
│   ├── about/             # About section
│   ├── contact/           # Contact section
│   ├── featured/          # Featured project entries
│   ├── hero/              # Hero section
│   ├── jobs/              # Work experience entries
│   ├── posts/             # Blog posts
│   └── projects/          # Project portfolio entries
├── src/
│   ├── components/        # React components
│   │   ├── sections/      # Page section components
│   │   └── icons/         # SVG icon components
│   ├── pages/             # Gatsby pages
│   ├── templates/         # Post and tag templates
│   ├── styles/            # Global styles, theme, mixins
│   ├── fonts/             # Custom fonts (Calibre, SFMono)
│   └── config.js          # Site configuration
├── gatsby-config.js       # Gatsby plugins and metadata
├── gatsby-node.js         # Dynamic page generation
└── package.json
```

## Installation & Setup

**Prerequisites:** Node.js v16 (see `.nvmrc`), npm or Yarn

1. Install the Gatsby CLI

   ```sh
   npm install -g gatsby-cli
   ```

2. Install and use the correct version of Node using [NVM](https://github.com/nvm-sh/nvm)

   ```sh
   nvm install
   ```

3. Install dependencies

   ```sh
   yarn
   ```

4. Start the development server

   ```sh
   npm start
   ```

   The site runs at `http://localhost:8000` with a GraphQL playground at `http://localhost:8000/___graphql`.

## Building for Production

1. Generate a full static production build

   ```sh
   npm run build
   ```

2. Preview the production build locally

   ```sh
   npm run serve
   ```

## Customization

All content is managed through Markdown files in the `content/` directory:

- **Add a project:** Create a new `.md` file in `content/projects/` or `content/featured/`
- **Add a blog post:** Create a new folder in `content/posts/` with an `index.md`
- **Update work experience:** Edit or add entries in `content/jobs/`
- **Update about/hero/contact:** Edit the corresponding Markdown files

Site metadata and plugin configs are in `gatsby-config.js`. Theme colors and fonts are defined in `src/styles/`.

## Color Reference

| Color          | Hex       |
| -------------- | --------- |
| Navy           | `#0a192f` |
| Light Navy     | `#172a45` |
| Lightest Navy  | `#303C55` |
| Slate          | `#8892b0` |
| Light Slate    | `#a8b2d1` |
| Lightest Slate | `#ccd6f6` |
| White          | `#e6f1ff` |
| Green          | `#64ffda` |

## License

MIT
