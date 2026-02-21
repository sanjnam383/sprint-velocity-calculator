# 📊 Sprint Velocity Calculator

> A PM tool to track sprint velocity, measure burnout risk, forecast next sprint, and get AI-powered coaching — deployed on Vercel. No backend. No database. 100% free.

🔗 **Live Demo:** [sprint-velocity-calculator-three.vercel.app](https://sprint-velocity-calculator-three.vercel.app)

---

## 📌 Why This Exists

Velocity data lives in Jira or spreadsheets but PMs rarely get a quick visual answer to: *"Is my team healthy? Are they burning out? What should I plan for next sprint?"*

This tool answers all three in under 30 seconds.

---

## ✅ Features

| Feature | Description |
|---------|-------------|
| **Sprint Labels** | Name each sprint (e.g. Sprint 12 — Feb) for real context |
| **Velocity Chart** | Line chart with average velocity overlay |
| **Burnout Risk Score** | 0–100 score based on variance and velocity drops |
| **Health Grade** | A/B/C/D grade combining trend + burnout + consistency |
| **Forecast Next Sprint** | 3-sprint moving average predicts next sprint velocity |
| **AI Insight** | Strict senior Agile PM analysis via Llama 3.3 70B |

---

## 🎯 How To Use

1. Enter story points for each sprint (optional: name each sprint)
2. Click **Calculate**
3. View health grade, burnout score, trend, and forecast
4. Optionally paste your OpenRouter API key for AI coaching

> **Tip:** Click **Load Sample** to see a demo instantly.

---

## 🔑 AI Insight

The AI feature uses **Llama 3.3 70B** via [OpenRouter](https://openrouter.ai) (free tier).

- Get a free API key at openrouter.ai
- Key is never stored — goes directly to OpenRouter
- Check "Remember for this session" to avoid re-pasting during the session

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| HTML / CSS / JS | Single file, no framework |
| Chart.js | Velocity trend chart |
| OpenRouter API | AI coaching (optional, free tier) |
| Vercel | Hosting and deployment |

**Cost: 100% Free**

---

## 📐 How the Scores Work

**Burnout Risk Score (0–100)**
Based on coefficient of variation (velocity variance) + number of sprint-to-sprint drops over 20%. Higher = more inconsistency = higher risk.

**Health Grade**
- **A (85–100):** Stable velocity, low burnout, positive or flat trend
- **B (70–84):** Minor inconsistencies, generally healthy
- **C (55–69):** Noticeable variance or declining trend — warrants attention
- **D (0–54):** High variance, burnout risk, or sharp decline — action needed

**Forecast**
3-sprint moving average of the most recent sprints. Simple and reliable for near-term planning.

---

## ⚠️ Current Limitations

- Forecast is a simple moving average — not predictive modelling
- No data persistence — refreshing the page clears inputs
- AI insight requires an OpenRouter API key from the user
- No multi-team comparison yet

---

## 🔮 Future Improvements

- [ ] Save and load sprint data (localStorage)
- [ ] Team capacity % field per sprint
- [ ] Export data as CSV
- [ ] Multi-team comparison on same chart
- [ ] Sprint notes field (e.g. "2 members on leave")

---

## 👩‍💻 Built By

**Sanjana M** — Turning PM chaos into clarity, one sprint at a time
