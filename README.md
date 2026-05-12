# Aditi Nayanar — Portfolio

Personal portfolio website. Live at: `https://Aditi-N-28.github.io/portfolio`

## How to deploy on GitHub Pages

1. Create a new repo on GitHub (e.g. `portfolio`)
2. Upload `index.html` to the repo root
3. Go to **Settings → Pages → Source → Deploy from branch → main / root**
4. Hit Save — your site goes live in ~1 minute

## How to update your portfolio

Open `index.html` in any text editor (VS Code recommended).

### Add a new project
Find the `<!-- PROJECTS -->` section and copy-paste this block:

```html
<div class="proj-card reveal">
  <div class="proj-head">
    <div class="proj-title">Your Project Title</div>
    <div class="proj-meta">
      <span class="badge badge-hack">Hackathon</span>  <!-- or badge-uni -->
      <span class="proj-date">Month Year</span>
    </div>
  </div>
  <div class="proj-desc">One or two sentences describing what you built and why it matters.</div>
  <div class="proj-tags">
    <span class="proj-tag">Tech 1</span>
    <span class="proj-tag">Tech 2</span>
  </div>
</div>
```

### Add a new skill tag
Find the right `.sk-card` block and add:
```html
<span class="sk-tag">New Skill</span>
```

### Add a new experience
Find `<!-- EXPERIENCE -->` and copy a `<div class="tl-item">` block.

### Update stats on the hero
Search for `hero-stats` and change the `.val` numbers.

### Update the typed phrases
Find `const phrases=` near the bottom `<script>` tag and edit the array.

## File structure
```
portfolio/
└── index.html   ← everything is in this one file
```

No build tools, no npm, no frameworks — just open in browser and edit.
