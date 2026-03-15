# Le Structureur — lestructureur.fr

## Stack
Static HTML/CSS/JS site hosted on Vercel. No build step, no framework.
Domain: lestructureur.fr (OVH DNS → Vercel)
GitHub: github.com/Lebmont27/lestructureur
Newsletter: lestructureur.substack.com
Analytics: Plausible (lestructureur.fr)

## Structure
index.html              — Homepage
a-propos.html           — About page
articles/*/index.html   — Article pages (one folder per article)
css/style.css           — Single stylesheet for entire site
images/                 — og-image.png, og-generator.html
data/                   — CSV templates for weekly market data articles

## Publishing workflow
1. Create article folder in articles/ with index.html
2. Add article card to index.html homepage grid
3. Add URL to sitemap.xml
4. git add, commit, push — Vercel auto-deploys on push to main

## Design
- Fonts: Playfair Display (headlines), DM Sans (body), JetBrains Mono (labels)
- Hero section: dark (#0a0a0f), rest of site: warm cream (#faf8f5)
- Accent: gold (#b8942e)
- CSS variables defined in :root of style.css

## Writing rules
- NEVER use dashes (-) in article text. Use commas, semicolons, periods.
- Tone: honest insider, educational, not salesy
- Author name: "Adrien" only (no last name)
- Bio: ancien structureur salle de marchés, now in direct distribution

## SEO
- Each page needs: canonical tag, og:image, JSON-LD (Article or WebSite)
- Google Search Console configured, sitemap submitted
- Target keywords: autocall, produit structuré, patrimoine, PEA
