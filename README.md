# Portfolio Workshop — Build Your Own Site with AI

This repo contains everything from today's workshop: the exact prompts, the Git commands, and the resources you need to build and deploy your own portfolio.

> Clone this repo, or just copy the sections below directly.

```bash
git clone <this-repo-url>
```

---

## 1. The Design Direction

We're building a **minimalist, editorial-style** portfolio — think design studio / print magazine, not a generic dark-mode developer template. Warm cream background, serif headings, one muted accent color, lots of whitespace. No neon gradients, no glassmorphism, no glowing dark dashboards.

---

## 2. The Two Prompts

Use these together. **Prompt 1** is the design and engineering spec — don't edit it. **Prompt 2** is where you add your own details.

### Prompt 1 — Design & Engineering Spec

```
You are a senior frontend engineer and brand designer, known for elegant,
editorial-quality personal websites — think a refined design studio's site,
not a typical "developer dark-mode dashboard" template.

DESIGN DIRECTION (follow this precisely):
- Aesthetic: minimalist, editorial, timeless — closer to a print magazine or
  an art gallery website than a SaaS dashboard.
- Background: warm off-white / cream (e.g. #F7F4EF), NOT pure white and NOT dark.
- Text: deep ink/charcoal (e.g. #1C1B19), never neon, never glowing text.
- Accent color: ONE muted, sophisticated tone only — pick one: warm terracotta,
  deep forest green, muted ochre/gold, or dusty clay. Use it sparingly
  (small text highlights, underlines, one button) — never as a full-section
  background or gradient.
- Typography: pair a classic serif display font (e.g. "Playfair Display",
  "Fraunces", or "Cormorant") for headings with a clean, neutral sans-serif
  (e.g. "Inter" or "Söhne"-style) for body text. Large, confident heading
  sizes with generous line-height. This typographic pairing is the most
  important part of the design — get it right.
- Layout: generous whitespace, wide margins, content in a centered readable
  column (max-width ~1100px), asymmetric but intentional grid for the
  projects section (not identical evenly-spaced cards).
- Dividers: thin hairline rules instead of boxed cards/heavy shadows.
- Motion: restrained — simple fade/slide-up on scroll only. No flashy
  gradients, no glassmorphism, no neon glow, no particle backgrounds,
  no dark-mode-by-default developer aesthetic.
- Explicitly AVOID: dark navy/black backgrounds with neon accent gradients,
  glassmorphism cards, glowing borders, "SaaS startup" hero patterns,
  generic Bootstrap-card project grids, and default AI-template look.

TECH STACK: React + Vite + Tailwind CSS. Framer Motion allowed only for
subtle fade/slide entrance animations — nothing flashy.

SECTIONS (in this order):
1. Hero — name, a short editorial-style tagline (not a generic "Full Stack
   Developer" label), a one-sentence intro, one understated CTA.
2. About — a short first-person bio paragraph.
3. Skills — presented as a clean inline list or minimal typographic grid,
   not colorful pill badges.
4. Projects — 3 entries, asymmetric editorial layout, each with title,
   one-line description, tech used, a "View" link and a "Live" link.
5. Experience/Education — simple vertical timeline, minimal styling,
   hairline connectors, no icons-in-circles cliché.
6. Contact — email, GitHub, LinkedIn as understated text links (not
   colorful icon buttons), a "Chat on WhatsApp" link, and a
   "Download Resume" link.

ENGINEERING REQUIREMENTS:
- Fully responsive: mobile, tablet, and desktop.
- Semantic HTML, proper heading hierarchy, alt text on all images,
  sufficient color contrast, keyboard-navigable.
- SEO: meta title, meta description, Open Graph tags.
- All personal content lives in ONE separate data file (e.g. data/portfolio.js)
  so it can be edited without touching component code.
- Clean folder structure: components/, data/, assets/.
- No build errors, no console warnings, deployment-ready for Vercel with
  zero extra config.

QUALITY BAR: Take the time needed to produce a genuinely polished,
professional-looking result — prioritize design quality and code
correctness over speed. A slower, better result is preferred.

Wait for my next message — it will contain my personal details to insert
into this design. Do not generate anything until you receive it.
```

### Prompt 2 — Your Details (fill this in yourself)

```
Here are my details to insert into the design above:

Name: [Your full name]
Tagline: [One editorial-style line, e.g. "Building thoughtful software, one project at a time"]
About (2–3 sentences, first person): [Your bio]

Skills: [e.g. React, Node.js, Python, PostgreSQL, Figma]

Projects:
1. [Project name] — [one-line description] — GitHub: [link] — Live: [link, or "N/A"]
2. [Project name] — [one-line description] — GitHub: [link] — Live: [link, or "N/A"]
3. [Project name] — [one-line description] — GitHub: [link] — Live: [link, or "N/A"]

Experience/Education (most recent first):
- [Role/Degree] — [Organization] — [Year(s)]
- [Role/Degree] — [Organization] — [Year(s)]

Contact:
Email: [your email]
GitHub: [your GitHub URL]
LinkedIn: [your LinkedIn URL]
WhatsApp: https://wa.me/[your number, country code, no + or spaces]
Resume: [link to a PDF, or say "use a placeholder /resume.pdf path"]

Accent color choice: [pick one: terracotta / forest green / ochre gold / dusty clay]

Now generate the complete portfolio using this content, following the
design spec exactly as given.
```

**How to submit:** If your AI tool supports multi-turn chat, paste Prompt 1 first, then Prompt 2. If it's a one-shot tool, merge both into a single message. Either way — **submit once and wait**. A good result can take 10–20 minutes. Don't regenerate halfway through.

---

## 3. Git Commands

First-time setup for a new project:
```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

Every time you make changes after that:
```bash
git add .
git commit -m "describe what changed"
git push
```

---

## 4. Deploy on Vercel

1. Go to vercel.com → sign in with GitHub
2. "Add New Project" → import your portfolio repo
3. Leave defaults (Vercel auto-detects Vite/React) → Deploy
4. Your site is live — every future `git push` auto-redeploys it

---

## 5. Resources

| Purpose | Link |
|---|---|
| Colors | coolors.co |
| Serif/sans font pairing | fonts.google.com |
| Icons (used sparingly) | lucide.dev, heroicons.com |
| Inspiration | godly.website, awwwards.com |
| Free images | unsplash.com, pexels.com |

---

## 6. What You Should Have by the End

- [ ] A React portfolio project running locally
- [ ] Code pushed to a public GitHub repo
- [ ] A live Vercel URL
- [ ] Both prompts saved for future projects

## 7. Homework

- Rewrite your About section fully in your own voice
- Add real project screenshots
- (Optional) connect a custom domain in Vercel
- Share your live link on LinkedIn

---

## Contact
— Name : Chethan KR <br>
— Gmail : chethankr.dev@gmail.com <br>
— Linkedin : www.linkedin.com/in/chethan-kr-dev <br>
— GitHub : https://github.com/Chethan814 <br>