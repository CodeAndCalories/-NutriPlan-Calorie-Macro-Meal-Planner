[README.md](https://github.com/user-attachments/files/25463743/README.md)
# 🥦 NutriPlan — Calorie & Macro Meal Planner

A free, offline, single-file meal planning web app you can run directly from GitHub Pages. No sign-up, no API keys, no internet connection required after the first load.

**[▶ Live Demo](https://your-username.github.io/nutriplan)** ← replace with your GitHub Pages URL

---

## ✨ Features

### 🎯 Calorie & Macro Targets
- Set goals **daily or weekly** — weekly mode auto-calculates the daily split
- Enter macros in **grams or percentages** (percentage mode validates they sum to 100)
- Covers protein, carbohydrates, and fat

### 🥗 Dietary Preferences
- High Protein, Vegetarian, Dairy Free, Gluten Free, Budget Friendly
- Optional **snack slot** per day
- **Exclude ingredients** by typing them as a comma-separated list (e.g. `nuts, shrimp, tofu`)

### 📅 7-Day Meal Plan
- Generates **3 meals per day** (+ optional snack) pulled from a built-in dataset of 90 meals
- Smart scoring picks meals that best match your calorie and protein targets
- **Lock individual meals** so regenerating won't replace ones you like
- **Regenerate a single day** or the **entire week** with one click
- Adjust **servings per meal** — all nutrition and grocery quantities update automatically
- Expandable **recipe panel** per meal with ingredients and step-by-step instructions

### 📊 Progress & Summary
- Per-day calorie progress bar with **On Track / Under / Over** status badge
- Weekly summary cards: total calories, daily average, protein, carbs, and fat

### 🛒 Grocery List
- Auto-generated from your full week plan
- Ingredients **combined across meals** (e.g. chicken breast from 4 meals = one line)
- Organized into categories: Produce, Protein, Dairy, Pantry, Spices, and more
- Scales with your servings settings
- **Copy to clipboard** or **download as .txt**
- Tap checkboxes to tick items off as you shop

### 💾 Persistent Storage
- Your plan and settings are saved to `localStorage` — survive page refreshes automatically

---

## 🍽️ Built-in Meal Dataset

| Category   | Count |
|------------|-------|
| Breakfasts | 25    |
| Lunches    | 25    |
| Dinners    | 25    |
| Snacks     | 15    |
| **Total**  | **90**|

Every meal includes: name, description, tagged dietary filters, structured ingredient list (with quantities and units), step-by-step instructions, and per-serving nutrition (calories, protein, carbs, fat).

---

## 🚀 Deploy to GitHub Pages in 3 Steps

1. **Fork or create** a new GitHub repository
2. **Upload** `meal-planner.html` to the root of the repo
3. Go to **Settings → Pages**, set the source to `main` branch and `/ (root)`, then save

Your planner will be live at:
```
https://your-username.github.io/repository-name/meal-planner.html
```

> **Tip:** Rename the file to `index.html` so the URL is cleaner:
> `https://your-username.github.io/repository-name/`

---

## 🛠️ Tech Stack

| Layer      | Details                          |
|------------|----------------------------------|
| HTML       | Semantic, accessible markup      |
| CSS        | Custom properties, responsive grid, no frameworks |
| JavaScript | Vanilla ES6+, no dependencies    |
| Storage    | Browser `localStorage`           |
| Fonts      | DM Serif Display + DM Sans (Google Fonts CDN) |

**Fully offline** after initial load (except for Google Fonts, which is optional — the app works without them using system fallback fonts).

---

## 📱 Responsive Design

Works on desktop, tablet, and mobile. On smaller screens the sidebar stacks above the main plan area.

---

## 🗂️ File Structure

```
nutriplan/
├── meal-planner.html   ← the entire app (rename to index.html for clean URLs)
└── README.md           ← this file
```

Everything lives in a single `.html` file — no build tools, no `node_modules`, no config files.

---

## 🔒 Privacy

All data stays on your device. Nothing is sent to any server. There are no analytics, no cookies (beyond localStorage), and no third-party trackers.

---

## 📝 License

MIT — free to use, modify, and share.

---

*Built with ❤️ and powered by vanilla HTML, CSS, and JavaScript.*
