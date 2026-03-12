Reproducible research project created using RMarkdown.

# Clash Royale Gameplay Statistical Analysis

![R](https://img.shields.io/badge/language-R-blue)
![Statistics](https://img.shields.io/badge/methods-Statistical%20Analysis-green)
![Status](https://img.shields.io/badge/project-Portfolio-orange)

## Project Overview

This project analyzes **30 days of Clash Royale gameplay data** using statistical techniques in **R**.  
The goal is to explore how **player mood and hours played influence match outcomes**.

The analysis includes:

- Data visualization
- Linear regression
- Binomial regression
- Hypothesis testing

---

## Dataset Description

Each row represents **one day of gameplay**.

Variables include:

- `Hours_Played`
- `Wins`
- `Losses`
- `Mood` (1–5 scale)
- `Matches_Played`

The dataset was manually recorded during daily gameplay sessions.

Dataset size: **30 observations**

---

## Statistical Question

**Does Mood Level 5 significantly increase the probability of winning compared to Mood Level 3 after controlling for Hours Played?**

---

## Key Result

The binomial regression model estimates:

- **Odds Ratio (Mood 5 vs Mood 3): 1.523**

Meaning:

Players in **Mood Level 5 have approximately 52% higher odds of winning** compared to Mood Level 3, holding hours played constant.

However, the p-value indicates that this effect is **not statistically significant at the 0.05 level**.

---

## Predicted Win Probability

At mean hours played:

| Mood Level | Win Probability |
|------------|----------------|
| 3 | 62% |
| 4 | 66% |
| 5 | 71% |

Higher mood levels are associated with higher predicted win probability.

---

## Visualization

![Win Probability by Mood](figures/mood_win_probability.png)

---

## Repository Structure
