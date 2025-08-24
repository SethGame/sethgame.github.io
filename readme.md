# sethgame.github.io

Personal blog and brain dump website for Seth Eom, built with Hugo and deployed to GitHub Pages.

## Overview

This is an English-language personal blog titled "Brain dump" where daily thoughts and experiences are documented ("Extracting daily thoughts from my brain and putting them into words"). The site follows a minimalist approach using the hugo-bearblog theme.

**Live Site:** https://sethgame.github.io/

## Technical Stack

- **Static Site Generator:** [Hugo](https://gohugo.io/)
- **Theme:** [hugo-bearblog](https://github.com/janraasch/hugo-bearblog)
- **Deployment:** GitHub Pages with automated CI/CD
- **Language:** English (en)
- **Content Format:** Markdown

## Project Structure

```
sethgame.github.io/
├── .github/
│   └── workflows/
│       └── gh-pages.yml          # GitHub Actions deployment workflow
├── hugo-site/                    # Hugo site root
│   ├── content/
│   │   ├── _index.md            # Homepage with author summary
│   │   ├── about.md             # Resume/CV page
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
- **Language:** English (`en`)
- **Author:** Seth Eom
- **Description:** Seth - Computer Engineering Student & AI Researcher
- **Pagination:** 5 posts per page
- **Summary Length:** 30 words

## About the Author

**Seth Eom** - Undergraduate Computer Engineering student at Purdue University with expertise in:
- AI/ML Technologies (PyTorch, Neural Networks, CUDA-based memory profiling)
- Programming Languages (Python, C Programming, MATLAB, SystemVerilog, Verilog)
- Hardware Design (FPGA, Digital System Design, Microprocessor Systems)
- Languages (Korean Conversational, Japanese Conversational, English Native)

**Current Experience:**
- Undergraduate Researcher at Guo Lab @ Purdue ECE (December 2024 - Present)
- Working on AI neural network-based boundary detection in image processing

**Education:**
- Bachelor of Science in Computer Engineering, Purdue University (Expected May 2026)
- GPA: 3.76, Dean's List and Semester Honors
- Study Abroad: CJS Summer Japanese Program, Nanzan University, Japan (2024)

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
- **Homepage Summary:** Author introduction and background on landing page
- **Recent Posts:** Homepage displays 5 most recent posts
- **Resume Page:** Comprehensive CV with education, experience, and skills
- **English Language Support:** Optimized for English content
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

- **Email:** eom.seth@gmail.com
- **Location:** Wexford, PA, USA
- **LinkedIn:** [linkedin.com/in/eomh](https://linkedin.com/in/eomh)