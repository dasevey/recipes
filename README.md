# Dave's Recipe Book

A personal recipe web app with serving scaler, hosted on GitHub Pages.

---

## Setup Instructions

### Step 1 — Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon → **New repository**
3. Name it something like `recipes`
4. Set it to **Public** (required for GitHub Pages)
5. Click **Create repository**

---

### Step 2 — Upload Your Files

Upload these two files to the root of your repo:
- `index.html`
- `recipes.json`

You can drag and drop them right into the GitHub web interface.

---

### Step 3 — Enable GitHub Pages

1. In your repo, go to **Settings** → **Pages**
2. Under **Source**, select **main** branch and **/ (root)**
3. Click **Save**
4. Your app will be live at: `https://YOUR-USERNAME.github.io/recipes`

It may take a minute or two to go live the first time.

---

### Step 4 — Create a Personal Access Token

This lets the app save new recipes back to GitHub.

1. Go to **GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)**
2. Click **Generate new token (classic)**
3. Give it a name like `recipe-app`
4. Check the **repo** scope
5. Click **Generate token**
6. **Copy the token** — you won't see it again!

---

### Step 5 — Configure the App

1. Open your app at the GitHub Pages URL
2. You'll see a setup bar at the top — fill in:
   - Your GitHub username
   - Your repo name (e.g. `recipes`)
   - Your personal access token
3. Click **Save Config**

The config is saved in your browser. You only need to do this once per device.

---

## Adding Recipes

Click the **+ Add Recipe** button. For ingredients, use this format (one per line):

```
ingredient name | tsp-per-base-serving | unit | cut | used-in
```

**Unit types:**
- `V` — volume (teaspoons internally, displays as tsp/tbsp/cups)
- `PC` — pieces (salmon fillets, cans, etc.)
- `CL` — cloves
- `GARNISH` — shows "to taste", not scaled

**Examples:**
```
olive oil | 3 | V | | Marinade
garlic | 1 | CL | minced | Base
salmon fillets | 1 | PC | | Main
cilantro | 0 | GARNISH | chopped | Garnish
```

---

## Editing Recipes Directly

You can edit `recipes.json` directly in GitHub's web editor anytime — works great on mobile too. Just navigate to the file in your repo and click the pencil icon.

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire web app |
| `recipes.json` | All your recipe data |
| `README.md` | These instructions |
