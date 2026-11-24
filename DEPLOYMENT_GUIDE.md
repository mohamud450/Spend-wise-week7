# Deployment Guide – step by step (for you to follow)

I can't log in to your GitHub or Netlify accounts, so these steps must be done by you. The project is already prepared for deployment.

## Part 1 – Readiness (already done)
- `index.html` is at the project root; all paths are relative; no build step is required.
- Open `index.html` locally first and check it works.

## Part 2 – GitHub repository
**Option A – website (easiest, no commands)**
1. Unzip `spendwise-week6.zip`. Open the `spendwise` folder.
2. On github.com click **+ → New repository**. Name it `spendwise`, choose **Public**, click **Create repository**.
3. Click **uploading an existing file**, drag in everything INSIDE the `spendwise` folder (`index.html`, `style.css`, `script.js`, `images`, `README.md`, `netlify.toml`, `.gitignore`). Do not drag the folder itself, or `index.html` ends up in a subfolder.
4. Write a commit message such as "Initial SpendWise upload" and click **Commit changes**.

**Option B – command line**
```
cd spendwise
git init
git add .
git commit -m "Initial SpendWise upload"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/spendwise.git
git push -u origin main
```

## Part 3 – Netlify deployment
1. Sign in at app.netlify.com (use **Log in with GitHub**).
2. **Add new site → Import an existing project → GitHub**, authorize Netlify, choose your `spendwise` repo.
3. Branch: `main`. Build command: leave empty. Publish directory: leave empty or `.`
4. Click **Deploy**. When it finishes you get a URL like `https://random-name-123.netlify.app`.

## Part 4 – Custom site name
**Site configuration → Site details → Change site name.** Choose something like `spendwise-yourname`. Your URL becomes `https://spendwise-yourname.netlify.app`. If the name is taken, try another.

## Part 5 – Continuous deployment test
1. In `index.html`, change the footer line  
   `<p>SpendWise &ndash; Week 6</p>`  
   to  
   `<p>SpendWise &ndash; Live on Netlify</p>`
2. On GitHub: open `index.html` → pencil icon (edit) → make the change → **Commit changes**. (Or `git add . && git commit -m "Update footer" && git push`.)
3. In Netlify open **Deploys**. A new deploy starts by itself. Wait for **Published**, then refresh your live site (Ctrl+Shift+R) and confirm the footer changed.
4. Take a screenshot of the Deploys list for your own records.

## Part 6 – Final testing checklist (on the live URL)
- [ ] Page loads with fonts, colors and the logo
- [ ] Set Budget updates the dashboard
- [ ] Add Expense works, and shows errors for empty fields
- [ ] Delete and Clear All Expenses work
- [ ] Category totals and status message change correctly
- [ ] YouTube video plays
- [ ] Open the browser console (F12): no red errors
- [ ] Test on your phone

## Finish
1. Put your live URL, repo URL and your own answers into every **[FILL IN]** in `README.md` and commit it.
2. Make sure the repo is **Public**.
3. Submit only the GitHub repository link in the LMS.
