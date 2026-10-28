# Ramya Kannan — Portfolio Site

A simple, dependency-free personal portfolio built with plain HTML, CSS, and JavaScript.

## Structure

```
portfolio/
├── index.html       Main page (About, Experience, Projects, Contact)
├── style.css        All styling (dark/techy theme)
├── script.js        Mobile nav toggle + scroll-reveal animations
└── assets/
    └── Ramya_Kannan_Resume.pdf
```

No build tools, no frameworks, no npm install — just open `index.html` in a browser to preview it locally, or deploy as-is.

## Editing content

- **Text/sections**: edit `index.html` directly. Each section is commented (`<!-- ===== About ===== -->`, etc.)
- **Colors/fonts/spacing**: edit the CSS variables at the top of `style.css` under `:root` — e.g. change `--accent: #5eead4;` to swap the accent color site-wide.
- **Resume**: replace `assets/Ramya_Kannan_Resume.pdf` with an updated file (keep the same filename, or update the links in `index.html` if you rename it).

## Deploying for free with GitHub Pages

1. Create a new GitHub repository (e.g. `ramseskannan.github.io` for a root-level URL, or any name for a project URL like `username.github.io/repo-name`).
2. Push this folder's contents to the repo:
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/ramseskannan/<your-repo-name>.git
   git push -u origin main
   ```
3. On GitHub: go to the repo's **Settings → Pages**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`, then Save.
4. Your site will be live at `https://ramseskannan.github.io/` (or `https://ramseskannan.github.io/<repo-name>/` for a project repo) within a minute or two.

### Custom domain (optional)

If you buy a domain later, add a `CNAME` file with just the domain name in it to the repo root, and point your domain's DNS at GitHub Pages per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Alternative hosts

Vercel and Netlify both support dragging and dropping a static folder (no GitHub required) if you want something even faster to get live — just upload this folder in their dashboard.
