# Ignvvcio254 👋

**Full Stack Developer** • Obsesivamente dedicado

---

## Skills

**Frontend**  
<img src="https://skillicons.dev/icons?i=react,angular,typescript,astro,html,css,tailwind" />

**Backend**  
<img src="https://skillicons.dev/icons?i=nodejs,python,fastapi,django,flask,dotnet" />

**Database**  
<img src="https://skillicons.dev/icons?i=mongodb,postgresql,mysql,supabase" />

**DevOps & Cloud**  
<img src="https://skillicons.dev/icons?i=aws,docker,git,linux,nginx" />

**Tools**  
<img src="https://skillicons.dev/icons?i=vscode,figma,androidstudio,discord" />

---

## Current Project

**[Portfolio 2.0](https://portafolio-254.vercel.app/)**

---

## Stats

<div align="center">
  
**Watch my contribution graph get eaten by the snake** 🐍

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Ignvvcio254/Ignvvcio254/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Ignvvcio254/Ignvvcio254/output/github-contribution-grid-snake.svg">
  <img alt="snake" src="https://raw.githubusercontent.com/Ignvvcio254/Ignvvcio254/output/github-contribution-grid-snake.svg">
</picture>

</div>

---

## 🐍 Setup Instructions

### 1. Create the Snake Animation Workflow

Create file: `.github/workflows/snake.yml`

```yaml
name: Generate snake animation
on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Generate snake animation
    runs-on: ubuntu-latest
    steps:
      # Snake Animation - automatically eats contributions
      - uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: Ignvvcio254
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark&color_snake=64b5f6&color_dots=#0d1117,#161b22,#21262d,#30363d,#64b5f6

      # Push to output branch
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### 2. Run the Workflow

1. Go to **Actions** tab in your repository
2. Click **"Generate snake animation"**
3. Click **"Run workflow"**
4. Wait for completion ✅

### 3. Result

The blue snake will **automatically move** and eat your contribution graph every 12 hours! 🎯.github/workflows/snake.yml`

```yaml
name: Generate snake game
on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: Ignvvcio254
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark&color_snake=64b5f6&color_dots=#0d1117,#161b22,#21262d,#30363d,#64b5f6

      # push the content to a branch
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### 2. Run the Workflow

1. Go to **Actions** tab in your repository
2. Click **"Generate snake game"**
3. Click **"Run workflow"**
4. Wait for completion ✅

### 3. Result

Your blue snake will be generated and the README will show your contribution graph being eaten! 🎯
