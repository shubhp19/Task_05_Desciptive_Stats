
# 📅 August 15 Prompts – LLM Evaluation

## Prompt 1
**"Can you create a bar chart showing the top 5 players by total points this season?"**

> **ChatGPT Response**:  
> A bar chart was successfully generated showing the top 5 scorers based on total points.

![Top 5 Players by Total Points](top_5_points_chart.png)

---

## Prompt 2
**"Based on this season’s data, who are the top 5 scorers on the team? Please rank them by total points scored."**

> **ChatGPT Response**:  

🏀 **Top 5 Players by Total Points Scored**

| Rank | Player               | Total Points |
|------|----------------------|---------------|
| 1    | J.J. Starling        | 764           |
| 2    | Eddie Lampkin Jr.    | 617           |
| 3    | Jyáre Davis          | 503           |
| 4    | Chris Bell           | 489           |
| 5    | Lucas Taylor         | 352           |

✅ **Correct** – Matches Python-calculated totals.

---

## Prompt 3
**"Using a custom impact formula that adds a player’s points, assists, and total rebounds, who are the top 5 most impactful players this season?"**

> **ChatGPT Response**:  

🔥 **Top 5 Most Impactful Players (PTS + Assists + Rebounds)**

| Rank | Player               | PTS | A   | TOT | Impact Score |
|------|----------------------|-----|-----|-----|---------------|
| 1    | Eddie Lampkin Jr.    | 617 | 109 | 533 | 1259          |
| 2    | J.J. Starling        | 764 | 125 | 160 | 1049          |
| 3    | Jyáre Davis          | 503 |  77 | 264 | 844           |
| 4    | Jaquan Carlos        | 332 | 208 | 114 | 654           |
| 5    | Chris Bell           | 489 |  21 | 96  | 606           |

✅ **Correct** – All values validated against dataset.

---

## Observations
- LLM returned accurate results for both structured and custom metric prompts.
- Visual and tabular outputs matched Python validations.
- Custom metric definition (PTS + A + TOT) was interpreted correctly without additional clarification.
