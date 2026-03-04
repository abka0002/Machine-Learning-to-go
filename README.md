# Machine Learning to Go

A collection of interactive web tools for understanding ML algorithms step by step.

🔗 **Live:** [machine-learning-to-go.netlify.app](https://machine-learning-to-go.netlify.app)

## Available Tools

| Tool | Topic | Link |
|------|-------|------|
| SMOTE & SMOTE-NC | Synthetic oversampling for imbalanced datasets | [Open](https://machine-learning-to-go.netlify.app/smote/) |

## Project Structure

```
├── index.html          ← Landing page with links to all tools
├── netlify.toml        ← Netlify config
├── smote/
│   └── index.html      ← SMOTE & SMOTE-NC interactive tool
├── <new-app>/          ← Future tools go here
│   └── index.html
└── README.md
```

## Adding a New Tool

1. Create a new folder (e.g. `regression/`)
2. Place your `index.html` inside it
3. Add a card linking to it in the root `index.html`
4. Push to GitHub — Netlify deploys automatically

## Deployment Guide

### Step 1 — Clone the repo

```bash
git clone https://github.com/abka0002/Machine-Learning-to-go.git
cd Machine-Learning-to-go
```

### Step 2 — Add the project files

Copy all downloaded files into the repo so it matches the structure above.

### Step 3 — Push to GitHub

```bash
git add .
git commit -m "Add ML tools with landing page"
git push origin main
```

### Step 4 — Connect Netlify

1. Go to [app.netlify.com](https://app.netlify.com/) and log in (free account).
2. Click **"Add new site"** → **"Import an existing project"**.
3. Choose **GitHub** and select **Machine-Learning-to-go**.
4. Set:
   - **Branch:** `main`
   - **Build command:** *(leave empty)*
   - **Publish directory:** `.`
5. Click **"Deploy site"**.

### Step 5 — Set a custom site name (optional)

Go to **Site configuration** → **Site details** → **Change site name** → enter `machine-learning-to-go`.

Your site will be live at `https://machine-learning-to-go.netlify.app`.

### Updating

Every `git push` triggers automatic redeployment.

## Tech Stack

Pure HTML / CSS / JavaScript — no build step required.
