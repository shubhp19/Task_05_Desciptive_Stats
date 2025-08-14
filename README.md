# 📊 Task_05_Descriptive_Stats

## 🧠 Research Task 05: Descriptive Statistics + LLM Evaluation

This project investigates how well a large language model (LLM) can interpret structured sports data and generate accurate insights using only natural language prompts. All LLM responses are validated using Python-based statistical analysis.

---

## 🏀 Dataset

- **Title**: Syracuse Men’s Basketball 2024–2025 Season
- **Format**: CSV (converted from Excel)
- **Size**: 32 rows × 16 players
- **Metrics Included**: Points (PTS), Rebounds (REB), Assists (AST), Minutes (MIN), FG%, GP-GS, and more

> ⚠️ Dataset is **not included** in the repo per instructions

---

## 🧮 Python Workflow

**File**: `python_phase2.ipynb`

Libraries used:
- `csv`, `statistics`, `collections`, `matplotlib`

Analysis performed:
- Overall summary stats (mean, std, min, max)
- Grouped stats by player
- Custom impact metric: `PTS + AST + REB`
- Visualization: bar chart for top scorers
- Data cleaning (fixed Excel-import formatting issues in GP-GS column)
- Bench player filtering (based on GP-GS threshold)

---

## 🤖 LLM Workflow

**LLM Used**: ChatGPT-4

### ✅ Phase 1 Prompts:
1. Who is the top scorer?
2. Who had the highest rebound average?
3. Who is the most consistent performer?

➡️ All answers were **correct or reasonable**, validated in Python

---

### ✅ Phase 2 Prompts (August 15):
1. Create a bar chart of the top 5 scorers
2. Rank top 5 players by total points
3. Use a custom formula: `PTS + AST + TOT` to find most impactful players
4. Identify a bench player to promote based on per-game performance
5. Discuss LLM limitations where game logs were missing

➡️ All answers were validated using Python  
➡️ LLM handled custom metrics and visualization tasks well

---

## 📈 Evaluation Summary

| Area                     | Performance                          |
|--------------------------|--------------------------------------|
| Top scorer ranking       | ✅ Correct                            |
| Rebound leader           | ✅ Correct                            |
| Consistency metric       | ✅ Reasonable interpretation          |
| Custom impact metric     | ✅ Correct (PTS + AST + REB)         |
| Visualization            | ✅ Matched chart from Python         |
| Edge cases + limitations | ✅ Identified and discussed          |

---

## 📂 Repository Files

```bash
├── python_stats-Copy1.ipynb       # Python validation code
├── llm_august15_prompts.md        # Prompts and LLM answers (Phase 2)
├── Research_Task_05 (1).docx      # Task write-up and reflections
├── README.md                      # This file
