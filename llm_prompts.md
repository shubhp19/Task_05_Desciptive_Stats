# 🧠 LLM Prompts & Responses – Task 05

## 🔍 Objective
To evaluate the ability of a large language model (LLM) to analyze structured sports data and return correct or reasonable insights when prompted in natural language.

---

## ✅ Dataset Used
- **Team**: Syracuse Men’s Basketball (2024–25 Season)
- **Format**: CSV (converted from Excel)
- **Records**: 32 rows, 16 players
- **Metrics**: Points, Rebounds, FG%, AVG_PTS, etc.

---

## 🤖 Tool Used
- **LLM**: ChatGPT-4 (OpenAI)
- **Mode**: Natural language prompting only (no code execution)

---

## 📥 Prompts Asked

### 1. "Who is the top scorer?"
> **LLM Answer**:  
> *"J.J. Starling with 463 total points."*  
> ✅ **Correct** – Matches Python analysis

---

### 2. "Which player had the highest rebound average?"
> **LLM Answer**:  
> *"Eddie Lampkin Jr. with an average of 10.8 rebounds per game."*  
> ✅ **Correct** – Matches `AVG_RB` column in data

---

### 3. "Give me the most consistent performer based on standard deviation of PTS"
> **LLM Answer**:  
> *"Lucas Taylor, whose scoring average (7.7 PPG) is closest to the team-wide average, making him the most statistically consistent player across games."*  
> ✅ **Reasonable** – Not exact std dev, but the answer reflects an approximation of consistency

---

## 🧠 Observations

- ChatGPT understood and correctly answered fact-based numerical queries.
- Interpretation-type queries (e.g. "most consistent") were approximated well even without direct access to code or computations.
- Prompt clarity impacts results — LLM performed better when asked simple and well-defined questions.
- Advanced queries requiring custom metrics may need iterative clarification or prompt engineering.

---

## 💡 Recommendations for Future Prompts

- When asking for "consistency", clarify using “lowest standard deviation of AVG_PTS”.
- For exploratory insights, chain questions: e.g., “Which player improved the most in scoring across games?”
- Use roleplay-based prompts: e.g., “You are a coach. Who would you focus on to improve offensive performance?”

---