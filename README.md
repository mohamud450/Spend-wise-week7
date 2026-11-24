# SpendWise

> **Before submitting:** every line marked **[FILL IN]** must be completed with your own information. Delete this note when you are done.

## Project Description
SpendWise is a personal budget and expense tracker. You set a monthly budget, add expenses with a name, amount, category and date, and the dashboard instantly shows your total spent, remaining balance, spending per category and a color-coded warning as you approach or pass your budget. You can delete single expenses or clear them all. The site also includes a collapsible help section and an embedded budgeting-tip video.

## Live Website
**Live Netlify URL:** [FILL IN – e.g. https://spendwise-yourname.netlify.app]

## Technologies Used
- **HTML5** – page structure, form, table, `<details>`, `<iframe>`
- **CSS3** – custom properties, grid and flexbox, Google Fonts (Young Serif, DM Sans), responsive layout
- **JavaScript (vanilla)** – variables, arrays, loops, conditionals, DOM manipulation, event listeners
- **Git & GitHub** – version control and source hosting
- **Netlify** – hosting with continuous deployment from GitHub

## GitHub Repository Information
- **Repository name:** [FILL IN – e.g. spendwise]
- **Repository URL:** [FILL IN – https://github.com/your-username/spendwise]
- **Visibility:** Public
- **Branch deployed:** `main`

### Project structure
```
spendwise/
├── index.html      # page structure
├── style.css       # all styling
├── script.js       # application logic
├── images/
│   └── logo.svg    # logo and favicon
├── netlify.toml    # Netlify settings (static site, no build)
├── .gitignore
└── README.md
```

## Deployment Process Summary
1. **Checked deployment readiness** – `index.html` is in the repository root, all file paths are relative, file names use matching lowercase, and the site works with no build step.
2. **Created a public GitHub repository** and uploaded the project files.
3. **Connected the repository to Netlify** (Add new site → Import an existing project → GitHub) and chose the `main` branch. Build command: none. Publish directory: the repository root.
4. **Renamed the site** in Site configuration → Change site name to [FILL IN – your chosen name], giving the URL above.
5. **Tested continuous deployment** – changed the footer text, committed and pushed to GitHub, and confirmed that Netlify rebuilt automatically and the live site showed the change. Update made: [FILL IN – e.g. footer changed to "SpendWise – Live on Netlify"]. Commit message: [FILL IN].
6. **Tested the live site** – checked that styles, fonts, the logo, the script (adding, deleting and clearing expenses, setting a budget) and the YouTube video all work on the live URL, on both desktop and mobile.

## Challenges Encountered During Deployment
[FILL IN – write about problems you really met. Examples of things that commonly happen, but only keep what is true for you:]
- [e.g. files uploaded inside a subfolder so Netlify showed "Page not found" until `index.html` was moved to the repository root]
- [e.g. changing the site name and the new URL being "already taken"]
- [e.g. the page not updating at first because the browser cached the old version]
- [e.g. a file-name case mismatch such as `Style.css` vs `style.css` that works locally but fails online]

## Lessons Learned
[FILL IN – in your own words, 3–4 sentences. Ideas: why Git commits matter; how continuous deployment saves time; why testing the live site matters even if it works locally; why relative paths and file-name case matter.]
