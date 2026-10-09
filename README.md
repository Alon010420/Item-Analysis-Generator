# 📊 Item Analysis Report Generator

> **A free, offline, browser-based tool for teachers to create professional Item Analysis Reports in minutes.**
> No Excel. No Word. No coding. Just type data → Generate → Print.

Created by **Jemmuel Alon** — Teacher, Philippines

---

## 🎯 What is this?

This is a **single-file HTML tool** that helps teachers generate a complete **Item Analysis Report** — the kind of report that usually takes hours to compute manually in Excel.

Teachers just need to:
1. **Type** their class data
2. **Click** Generate
3. **Print** or Save as PDF

Everything else — mean, median, mode, standard deviation, passing rate, mastery levels, donut charts, bar charts, recommendations — is **auto-computed**.

---

## ✨ Features

### 📊 Two Modes
- **Score + Topics Mode** — If you only have total scores per student (no per-item data). Still shows topic coverage + class performance.
- **Full Item Analysis Mode** — If you have per-item record (how many students got item #1, #2, #3 correct). Complete item analysis with mastery levels.

### 🧮 Auto-Computed Statistics
- Passing Rate
- Mean, Median, Mode
- Highest, Lowest
- Standard Deviation
- Range
- Score Distribution (buckets of 5)
- Mastery Levels: **Mastered** (≥75%), **Least Mastered** (50–74%), **Not Mastered** (<50%)

### 📈 Visual Reports
- **Pass / Fail donut chart**
- **Score distribution bar chart**
- **Mastery summary donut**
- **Top 10 hardest items** (Full Mode)
- **Color-coded item table** with remarks

### 🎨 Professional Design
- DepEd-style formal report layout
- Navy + gold color scheme
- Print-ready (A4, Letter, Long/Folio, Legal, A3, A5)
- Auto-saves data in browser (`localStorage`)

### 🛡️ Bulletproof Input
- Accepts scores in **any format** — newlines, commas, spaces, semicolons
- Auto-cleans weird characters
- Friendly error messages (Tagalog/Bisaya)
- Toast notifications (no annoying pop-ups)

### 📄 Paper Size Support
| Size | Dimensions | Notes |
|---|---|---|
| A4 | 210 × 297 mm | Default |
| Letter / Short | 8.5 × 11 in | |
| **Long / Folio** | **8.5 × 13 in** | PH long bond |
| Legal | 8.5 × 14 in | |
| A3 | 297 × 420 mm | Landscape |
| A5 | 148 × 210 mm | Landscape |

---

## 🚀 How to Use

### Option 1: Use Online (easiest)

**[👉 Click here to open the generator](https://YOUR-USERNAME.github.io/YOUR-REPO/report-generator.html)**

*(Replace with your actual GitHub Pages link after enabling it.)*

### Option 2: Use Offline

1. **Download** `report-generator.html`
2. **Double-click** the file → opens in any browser
3. Works even without internet (after first load)

### Option 3: Run from Source

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
# Then just open report-generator.html in your browser
```

---

## 📖 Step-by-Step Usage

### Step 1: Choose Mode
- **Score + Topics** — if you only have total scores
- **Full Item Analysis** — if you have per-item data

### Step 2: Fill School Info
School name, address, teacher name, grade & section, subject, term.

### Step 3: Exam Info
- Total items (e.g., 50)
- Passing score (e.g., 25)

### Step 4: Enter Student Scores
One score per line, or comma-separated:

```
45
46
48
42
49
```

Also works: `45, 46, 48, 42, 49`

### Step 5: Enter Topics (Optional in Score Mode)

**Full Mode:** `Topic, Number of Correct`
```
Digestive tract organ, 25
Digestive process, 29
Xylem and phloem, 24
```

**Score Mode:** Just the topic name
```
Digestive tract organ
Digestive process
Xylem and phloem
```

### Step 6: Generate & Print
- Click **Generate Report**
- Choose **Paper Size**
- Click **Print / Save as PDF**

---

## ⚠️ IMPORTANT — For Colored Print Output

Browsers **don't print colors by default** to save ink. To get colored output:

### In the Print Dialog:
1. Click **"More settings"** (or "Show more options")
2. ✅ Check **"Background graphics"**
3. ❌ Uncheck **"Headers and footers"**
4. Click **Print** or **Save as PDF**

**Note:** You only need to do this **once** — Chrome remembers your choice.

---

## 🖨 Sample Workflow

```
Exam → Check papers → Tally per item → Open generator → 
Type data → Generate → Print → Save PDF → Submit
```

**Tip for future Full Item Analysis:**
While checking papers, use a **tally sheet** like this:

```
Student    | 1 | 2 | 3 | 4 | 5 |...| 50 | TOTAL
───────────────────────────────────────────────
Juan       | ✓ | ✗ | ✓ | ✓ | ✗ |...|    | 41
Maria      | ✓ | ✓ | ✓ | ✗ | ✓ |...|    | 46
...
───────────────────────────────────────────────
CORRECT:   | 25| 29| 27| 30| 21|...|
```

The **bottom row (CORRECT)** is what you type in Step 5.

---

## 🧑‍💻 Tech Stack

- **HTML5** — single file, no build tools
- **CSS3** — custom properties, flexbox, grid, conic-gradient
- **Vanilla JavaScript** — no frameworks, no libraries
- **Google Fonts** — Inter + Playfair Display
- **localStorage** — auto-save feature

**Zero dependencies. Zero installation.**

---

## 📁 File Structure

```
item-analysis-generator/
├── report-generator.html    ← The whole app (single file)
├── README.md                ← This file
└── LICENSE                  ← MIT License
```

---

## 🌐 Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings** → **Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** → **/ (root)**
5. Click **Save**
6. Wait ~1 minute
7. Your link: `https://YOUR-USERNAME.github.io/YOUR-REPO/report-generator.html`

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repo
2. Create your branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 🐛 Known Issues / Limitations

- **Print colors** — requires manual "Background graphics" checkbox in print dialog (browser limitation)
- **LocalStorage** — data is saved in the browser, not synced across devices
- **No cloud sync** — everything is client-side; nothing is uploaded anywhere
- **Full Item Analysis** — requires manual tally sheet; the tool cannot magically know per-item data from total scores alone

---

## 📜 License

This project is licensed under the **MIT License** — free for personal and commercial use.

See [LICENSE](LICENSE) file for details.

---

## 👨‍🏫 About the Developer

**Jemmuel Alon**
Teacher · Philippines

> "I built this so teachers don't have to spend hours in Excel computing the same thing over and over. Type data, click, print. Done."

- GitHub: [@YOUR-USERNAME](https://github.com/YOUR-USERNAME)
- Email: your.email@example.com

---

## 🙏 Acknowledgements

- Department of Education (DepEd) Philippines — for the report format inspiration
- All teachers who gave feedback and tested this tool
- Open source community — for the tools that make projects like this possible

---

## 📸 Screenshots

### Input Screen
![Input Screen](screenshots/input.png)

### Generated Report
![Report](screenshots/report.png)

### Printed Output
![Print](screenshots/print.png)

*(Add your own screenshots to a `screenshots/` folder.)*

---

## ⭐ Support

If this tool helped you, please:
- ⭐ **Star** this repository
- 🐦 **Share** with fellow teachers
- 🐛 **Report** bugs or suggest features via [Issues](https://github.com/YOUR-USERNAME/YOUR-REPO/issues)

---

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/YOUR-USERNAME/YOUR-REPO?style=social)
![GitHub forks](https://img.shields.io/github/forks/YOUR-USERNAME/YOUR-REPO?style=social)
![GitHub issues](https://img.shields.io/github/issues/YOUR-USERNAME/YOUR-REPO)

---

**Made with ❤️ for Filipino teachers 🇵🇭**