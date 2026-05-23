# DevCard — 2-Hour AI-Assisted Capstone

Build and deploy your own **personal developer portfolio** in 2 hours using AI as your pair programmer. By the end you'll have a **live URL** you can share on LinkedIn and your CV.

---

## What You'll Build

A single-page portfolio with:
- **Hero section** — your name, title, photo, short tagline
- **About Me** — 2–3 sentence bio
- **Skills** — list/grid of technologies you know
- **Projects** — 2–3 cards (title, description, link)
- **Contact** — email + social links
- **One JS feature** — dark mode toggle (minimum), bonus features encouraged

Deployed live via **GitHub Pages**.

---

## What You Need
- A GitHub account
- VS Code (or any code editor)
- Git installed
- Access to an AI assistant (ChatGPT, Copilot, Claude, Gemini — any)
- A profile photo (optional but nice)

---

## Timeline (2 hours)

| Time | Phase | Goal |
|---|---|---|
| 0:00 – 0:10 | **Setup** | Create repo, clone locally, open in VS Code |
| 0:10 – 0:35 | **HTML** | Prompt AI to scaffold semantic structure, commit |
| 0:35 – 1:05 | **CSS** | Style it — colors, layout, responsive, commit |
| 1:05 – 1:35 | **JavaScript** | Add dark mode + 1 bonus feature, commit |
| 1:35 – 1:50 | **Deploy** | Push to GitHub, enable Pages, get live URL |
| 1:50 – 2:00 | **Show & Tell** | Share your live URL in the group chat |

> **Rule:** Commit at the end of every phase with a clear message. That's 4 minimum commits.

---

## Step-by-Step

### Phase 1 — Setup (10 min)
1. On GitHub, create a new public repo named `devcard` (no README, no .gitignore).
2. In your terminal:
   ```bash
   mkdir devcard && cd devcard
   git init
   echo "# DevCard" > README.md
   touch index.html styles.css script.js
   git add .
   git commit -m "Initial project structure"
   git branch -M main
   git remote add origin https://github.com/<your-username>/devcard.git
   git push -u origin main
   ```

### Phase 2 — HTML (25 min)
Prompt the AI to generate the structure. **Use the prompt patterns below.** Paste the result into `index.html`, review it, tweak it with your real info.

Commit:
```bash
git add . && git commit -m "Add HTML structure" && git push
```

### Phase 3 — CSS (30 min)
Prompt the AI to style it. Iterate: ask for a color palette, then layout, then responsiveness. Don't accept the first draft — refine.

Commit:
```bash
git add . && git commit -m "Add styling and responsive layout" && git push
```

### Phase 4 — JavaScript (30 min)
Add at least a **dark mode toggle**. Pick one bonus:
- Typing animation on the hero tagline
- Filter project cards by skill tag
- Contact form with validation
- Smooth scroll on nav links

Commit:
```bash
git add . && git commit -m "Add dark mode toggle and JS interactivity" && git push
```

### Phase 5 — Deploy (15 min)
1. On GitHub → your repo → **Settings** → **Pages**
2. Under **Source**, pick **Deploy from a branch** → `main` → `/ (root)` → **Save**
3. Wait ~1 minute, refresh — your live URL appears at the top:
   `https://<your-username>.github.io/devcard/`
4. Open it. Test on your phone too.

---

## Prompt Engineering Cheat Sheet

AI gives better output when you give it **role, context, constraints, and format**.

### Pattern: ROLE → TASK → CONSTRAINTS → FORMAT

> "Act as a **senior front-end developer**. Generate **semantic HTML5** for a personal portfolio page with these sections: hero, about, skills, projects, contact. Use proper landmarks (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`). No inline styles. Include placeholder text I can replace. Return only the code in one block."

### Starter Prompts

**HTML scaffold**
> Act as a senior front-end developer. Create semantic HTML5 for a one-page developer portfolio. Sections: hero (name, title, tagline, photo), about, skills (grid of 6), projects (3 cards with title/description/link), contact (email + GitHub + LinkedIn). Use semantic tags. Add class names I can style. Return only the HTML.

**CSS styling**
> Style this HTML with modern, mobile-first CSS. Use a dark navy + accent color palette, system font stack, CSS Grid for the projects section, Flexbox for the nav. Add subtle hover effects on cards and buttons. Make it responsive at 768px and 480px breakpoints. Here is the HTML: [paste]

**Dark mode toggle**
> Write vanilla JavaScript for a dark mode toggle button. It should: (1) toggle a `dark` class on `<body>`, (2) persist the choice in localStorage, (3) apply the saved choice on page load. Also give me the CSS variables setup for light and dark themes. Keep it minimal — no libraries.

**Debugging**
> My dark mode toggle isn't persisting after refresh. Here's my HTML, CSS, and JS: [paste]. What's wrong and how do I fix it? Explain the fix briefly.

**Refactor**
> Refactor this CSS to use CSS custom properties (variables) for colors and spacing so it's easier to theme. Keep the same visual output. [paste]

### Prompting Do's and Don'ts

| Do | Don't |
|---|---|
| Give the AI your existing code | "Make me a website" |
| Specify the stack (vanilla JS, no frameworks) | Accept the first answer blindly |
| Ask **why** when it suggests something | Paste secrets/API keys |
| Iterate in small steps | Ask for everything at once |
| Read the code before pasting it in | Skip understanding — you'll get stuck later |

---

## Submission Checklist

- [ ] Repo is public on GitHub
- [ ] At least 4 commits with clear messages
- [ ] Site is live on GitHub Pages
- [ ] Works on mobile (test in DevTools or your phone)
- [ ] Dark mode toggle works and persists
- [ ] README.md has your name + live URL
- [ ] Shared live URL in group chat

---

## Stretch Goals (if you finish early)

- Add a custom favicon
- Add a downloadable CV button
- Animate sections in on scroll (Intersection Observer)
- Add a custom domain
- Lighthouse score above 90 on all categories

---

**Have fun. Ship something. Share it.**
