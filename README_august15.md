
# 📊 Task 05: Descriptive Stats & LLM Evaluation – August 15 Update

This update builds upon the initial July 31 submission by integrating advanced metrics, visualizations, and expanded LLM prompt validation. The goal was not only to extract performance insights from the Syracuse Men's Basketball dataset but also to critically assess how well a large language model (ChatGPT-4) can reason over structured numeric data.

---

## 🧠 Phase 2 Goals

- Develop **custom metrics** to simulate coaching-level decisions.
- Test LLM’s ability to reason using **derived statistics** (not just raw facts).
- Visualize key player insights.
- Compare ChatGPT answers with Python-calculated values.

---

## 🧮 New Python Additions

- **Game Changer Index**: PTS + A + TOT (points + assists + total rebounds)
- **Top 5 Player Scoring Summary** with automated ranking
- **Bar Chart**: Visual visualization of top scorers
- **Grouped analysis** by player for advanced stat calculation
- **Data integrity fixes**: Converted `FG-FGA`, `FT-FTA`, `3FG-FGA` fields, ensured numeric types
- **Impact Ranking**: Sorted player contributions by custom metric

---

## 📥 Prompts Added to LLM Evaluation

| Prompt | Topic | Model Accuracy |
|--------|-------|----------------|
| "Top 5 players by total points?" | Scoring | ✅ Accurate |
| "Bar chart of top 5 scorers?" | Visualization | ✅ Accurate |
| "Top 5 most impactful players (PTS + A + TOT)?" | Custom Metric | ✅ Accurate |

All values provided by ChatGPT were validated against the Python-calculated outputs.

---

## 📌 Summary

This phase demonstrated that:

- ChatGPT handled **factual and derived stat queries** very well.
- Visual outputs (like bar charts) aligned with computed results.
- The LLM needed clear metric definitions but adapted well to **custom logic** when prompted.
- Using LLMs for sports insight is promising, especially with structured guidance.

---

## 📁 Files

- `python_stats-Copy1.ipynb` – Expanded stat analysis & custom metric code
- `llm_august15_prompts.md` – August prompt set and responses
- `README.md` – Project summary and progress
