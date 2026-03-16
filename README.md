# TU ODEOL Course Workload Estimator

**Tuskegee University — Office of Distance Education & Online Learning (ODEOL)**

A Carnegie Unit-compliant, browser-based Time-on-Task calculator for faculty developing online, blended, and face-to-face courses. Generates a branded print-to-PDF audit report for ODEOL records and Quality Matters review.

---

## Live URL (once deployed)

```
https://drntamm.github.io/tu-workload-estimator/
```

---

## Features

- Seven activity types: Reading, Video/Lecture, Writing, Quiz/Exam, Discussion, Project/Lab, Other
- Research-based time estimates (Rice University / Wake Forest Workload Estimator, Barre & Esarey, 2016)
- Live Carnegie Unit compliance gauge — adjusts dynamically by credit hours **and** term length
- One-click **Print / Save Audit Report** — opens browser print dialog; save as PDF
- Zero external dependencies — no CDN, no libraries, no backend
- Works in GitHub Pages, Canvas LMS embed, and all modern browsers

---

## File Structure

```
tu-workload-estimator/
├── index.html          ← The complete application
├── canvas-embed.html   ← Paste into Canvas HTML editor
└── README.md           ← This file
```

---

## Deployment

### Step 1 — GitHub Pages

1. Go to github.com and sign in as **drntamm**
2. Click **New repository** → name it exactly: `tu-workload-estimator`
3. Set visibility to **Public**
4. Click **Create repository**
5. Click **uploading an existing file** → drag and drop all three files
6. Click **Commit changes**
7. Go to **Settings → Pages**
8. Under **Source**: select `Deploy from a branch` → `main` → `/ (root)` → **Save**
9. Live at: `https://drntamm.github.io/tu-workload-estimator/`

---

### Step 2 — Canvas LMS Embed

1. Open the Canvas Page where you want the tool
2. Click **Edit** → click the **HTML Editor** button (`< >`)
3. Paste the entire contents of `canvas-embed.html` into the editor
4. Click **Save**

The page will show a branded banner, a launch button, and an inline iframe with the full tool.

> If Canvas restricts iframes on your instance, the launch button (opens in new tab) always works as a fallback.

---

## Estimation Methodology

| Activity | Basis |
|---|---|
| Reading | Words per minute by page density × reading purpose |
| Video / Lecture | Direct duration × format multiplier |
| Writing | Minutes per page by genre × drafting level (Torrance, 2013) |
| Quiz / Exam | Minutes per question type + study time |
| Discussion | Post length + peer response time |
| Project / Lab | Faculty-estimated hours |
| Other | Free-form faculty estimate |

Weekly Carnegie standard = (Credit Hours × 45) ÷ Term Weeks

---

*Tuskegee University is accredited by SACSCOC. www.tuskegee.edu*
