# sethgame.github.io

Personal blog and brain dump website for Jaesung Eom, built with Hugo and deployed to GitHub Pages.

## Overview

This is a Korean-language personal blog titled "Brain dump" (일상다반사를 뇌안에서 꺼내서 적고 바라보기) where daily thoughts and experiences are documented. The site follows a minimalist approach using the hugo-bearblog theme.

**Live Site:** https://sethgame.github.io/

## Technical Stack

- **Static Site Generator:** [Hugo](https://gohugo.io/)
- **Theme:** [hugo-bearblog](https://github.com/janraasch/hugo-bearblog)
- **Deployment:** GitHub Pages with automated CI/CD
- **Language:** Korean (ko)
- **Content Format:** Markdown

## Project Structure

```
sethgame.github.io/
├── .github/
│   └── workflows/
│       └── gh-pages.yml          # GitHub Actions deployment workflow
├── hugo-site/                    # Hugo site root
│   ├── content/
│   │   ├── _index.md            # Homepage content
│   │   ├── about.md             # About page
│   │   └── blog/                # Blog posts directory
│   │       ├── _index.md
│   │       └── *.md             # Individual blog posts
│   ├── layouts/
│   │   └── shortcodes/          # Custom Hugo shortcodes
│   ├── static/
│   │   └── CNAME                # Custom domain configuration
│   ├── themes/
│   │   └── hugo-bearblog/       # Theme submodule
│   └── hugo.toml                # Hugo configuration
├── .gitmodules                  # Git submodules configuration
└── readme.md                    # This file
```

## Site Configuration

- **Base URL:** `https://sethgame.github.io/`
- **Language:** Korean (`ko`)
- **Author:** Jaesung Eom
- **Description:** Personal brain dump blog
- **Pagination:** 5 posts per page
- **Summary Length:** 30 words

## About the Author

**Jaesung Eom** - Research Engineer at Autodesk with expertise in:
- Numerical Computing (Iterative solvers, FEM, Meshless methods)
- AI/ML Prototyping (LangChain, LangGraph, Azure OpenAI, AWS Bedrock)
- Programming Languages (Python, C/C++, FORTRAN, Golang, Rust)

**Education:**
- Ph.D. in Mechanical Engineering, KAIST (2007)
- M.S. in Mechanical Engineering, KAIST (2000)
- B.S. in Mechanical Engineering, KAIST (1998)

## Development Setup

### Prerequisites
- [Hugo](https://gohugo.io/installation/) (latest version)
- [Git](https://git-scm.com/)

### Local Development

1. **Clone the repository:**
   ```bash
   git clone --recurse-submodules https://github.com/sethgame/sethgame.github.io.git
   cd sethgame.github.io
   ```

2. **Navigate to Hugo site directory:**
   ```bash
   cd hugo-site
   ```

3. **Start local development server:**
   ```bash
   hugo server -D
   ```
   Site will be available at `http://localhost:1313`

4. **Build for production:**
   ```bash
   hugo --minify
   ```

### Adding New Content

1. **Create a new blog post:**
   ```bash
   cd hugo-site
   hugo new blog/YYYY-MM-DD-post-title.md
   ```

2. **Edit the front matter and content:**
   ```yaml
   ---
   title: "Your Post Title"
   date: 2025-01-XX-XX-XX+09:00
   draft: false
   slug: your-post-slug
   ---
   
   Your content here...
   ```

3. **Preview locally:**
   ```bash
   hugo server -D
   ```

## Deployment

The site is automatically deployed to GitHub Pages using GitHub Actions:

- **Trigger:** Push to `main` branch
- **Build:** Hugo with minification
- **Deploy:** Using official GitHub Pages actions
- **Custom Domain:** `sethgame.github.io` (via CNAME file)
- **Environment:** github-pages with proper permissions

The deployment workflow:
1. Checks out repository with submodules
2. Sets up Hugo (latest version)
3. Builds site with minification
4. Configures GitHub Pages environment
5. Uploads build artifacts
6. Deploys using official GitHub Pages action

## Features

- **Responsive Design:** Mobile-friendly hugo-bearblog theme
- **Recent Posts:** Homepage displays 5 most recent posts
- **Korean Language Support:** Optimized for Korean content
- **Custom Shortcodes:** Enhanced content capabilities
- **SEO Optimized:** Built-in SEO features from hugo-bearblog
- **Fast Loading:** Minimalist design and optimized assets

## Content Strategy

The blog follows a "1/100" approach, documenting daily thoughts and experiences as a personal knowledge repository. Content includes:
- Personal reflections and observations
- Technical insights and learning notes
- Embedded content from external sources (Notion, etc.)

## License

This project is personal content. The hugo-bearblog theme is licensed under its respective license.

## Contact

- **Email:** jaesung.eom@gmail.com
- **Location:** Pittsburgh, PA, USA