# Assignment 2: Understanding Labor Market Flows

**Course:** Labor Policy and the Future of Work
**Connects to:** Week 3 - Labor Market Dynamics and Search
**Due Date:** [To be determined]
**Points:** 75

---

## Overview

Labor economists distinguish between **stocks** (like the unemployment rate at a point in time) and **flows** (like the number of people hired or fired each month). This assignment uses data from the Job Openings and Labor Turnover Survey (JOLTS) to understand how workers move into and out of employment, and what these flows tell us about labor market conditions.

**Data is provided** - you don't need to download anything from BLS.

---

## Learning Objectives

By completing this assignment, you will:

1. Distinguish between stock and flow measures of the labor market
2. Understand what quits, layoffs, and job openings tell us about economic conditions
3. Create clear data visualizations and interpret cyclical patterns
4. Apply labor market search theory to real-world data
5. Write a concise policy analysis based on empirical evidence

---

## Background: Why Flows Matter

The unemployment rate tells you how many people are unemployed, but not *why* or *how quickly* things are changing. JOLTS data reveals:

- **Hires:** Workers added to payrolls (shows labor demand)
- **Quits:** Workers who voluntarily leave (shows worker confidence)
- **Layoffs:** Workers involuntarily separated (shows employer distress)
- **Job Openings:** Unfilled positions (shows unmet labor demand)

**Key insight:** Quits are "procyclical" (high in good times, low in bad times) because workers only quit when they're confident they can find something better. Layoffs are "countercyclical" (high in bad times).

---

## The Data

Download the dataset from [course LMS]: **`jolts_data_2001_2024.csv`**

This file contains monthly JOLTS data for the total nonfarm sector with the following variables:

| Variable | Description |
|----------|-------------|
| `date` | Month-year |
| `hires_rate` | Hires as % of employment |
| `quits_rate` | Quits as % of employment |
| `layoffs_rate` | Layoffs as % of employment |
| `openings_rate` | Job openings as % of employment |
| `unemployment_rate` | From BLS (for Beveridge Curve) |
| `recession` | 1 if NBER recession month, 0 otherwise |

---

## Part 1: Visualizing Labor Market Flows (25 points)

### Task 1.1: Quits vs. Layoffs Over Time

Create a **time-series graph** showing:
- Quit rate (one line)
- Layoff rate (another line)
- Date range: January 2001 to present
- Shade recession periods (use the `recession` variable)

**Requirements:**
- Clear title and axis labels
- Legend identifying each line
- Different colors for quits vs. layoffs
- Vertical line or annotation marking March 2020 (COVID onset)

You may use Excel, Google Sheets, R, Python, or any software you're comfortable with.

**Deliverable:** Your graph (PNG or PDF)

### Task 1.2: Interpretation (1 page)

Looking at your graph, answer:

**A.** Which rate is more volatile - quits or layoffs? Approximately what range does each fluctuate within?

**B.** Describe what happened to both rates during:
- The 2008-2009 recession
- The COVID shock (March-April 2020)
- The "Great Resignation" period (2021-2022)

**C.** In your own words, explain why quits are procyclical (high in good times) and layoffs are countercyclical (high in bad times). Connect this to worker bargaining power and job search theory from class.

---

## Part 2: The Beveridge Curve (25 points)

The **Beveridge Curve** shows the relationship between job openings and unemployment. It's named after British economist William Beveridge.

### Task 2.1: Create the Beveridge Curve

Create a **scatter plot** showing:
- X-axis: Unemployment rate
- Y-axis: Job openings rate
- Each point is one month of data

**Color-code by time period:**
- Blue: 2001-2007 (pre-Great Recession)
- Red: 2008-2019 (post-Great Recession)
- Green: 2020-present (COVID and after)

**Deliverable:** Your Beveridge Curve graph (PNG or PDF)

### Task 2.2: Interpretation (1 page)

**A.** Describe the general shape of the Beveridge Curve. Is the relationship between unemployment and job openings positive or negative? Why does this make economic sense?

**B.** Notice that the curve appears to have "shifted" over time. Specifically:
- Compare where the blue dots (2001-2007) cluster vs. the green dots (2020+)
- Are recent observations to the upper-right of older observations?

**C.** An "outward shift" of the Beveridge Curve means that for any given unemployment rate, there are more unfilled jobs than before. This suggests **reduced matching efficiency** - employers and workers are having trouble finding each other.

What might explain reduced matching efficiency in the 2020s? Propose at least two explanations. (Consider: skill mismatches, geographic mismatches, changed worker preferences, remote work, childcare, etc.)

---

## Part 3: Policy Memo (25 points)

Write a **2-page policy memo** addressed to the Secretary of Labor analyzing current labor market conditions based on JOLTS data.

### Required Sections:

**1. Executive Summary (1 paragraph)**
- Current state of the labor market in 2-3 sentences
- Your main policy recommendation

**2. Analysis of Current Conditions (1 page)**
Using the most recent data (2024), assess:
- Is the labor market currently "tight" (lots of openings, high quits) or "slack" (few openings, low quits)?
- How do current quit and layoff rates compare to historical averages?
- What does the Beveridge Curve position suggest about matching efficiency?

**3. Policy Recommendation (half page)**
Based on your analysis, recommend ONE policy priority:

*If the labor market is tight:*
- Policies to increase labor supply (immigration, childcare, training)
- Whether the Fed should continue tightening

*If the labor market is slack:*
- Active labor market policies (job search assistance, hiring subsidies)
- Whether unemployment insurance should be adjusted

**4. Limitations (1 paragraph)**
What can't JOLTS data tell us? What additional information would strengthen your analysis?

### Memo Format Requirements:
- Professional memo header (To, From, Date, Re:)
- 12pt font, 1-inch margins
- Bullet points are acceptable for key findings
- Cite your data source (BLS JOLTS)

---

## Submission Requirements

Submit via [course LMS]:

1. **Graph 1:** Quits vs. Layoffs time series
2. **Graph 2:** Beveridge Curve scatter plot
3. **Written document** containing:
   - Part 1.2 interpretation (1 page)
   - Part 2.2 interpretation (1 page)
   - Part 3 policy memo (2 pages)
   - Total: 4 pages plus graphs

**File naming:** `LastName_FirstName_Assignment2.pdf`

---

## Grading Rubric

| Component | Points | Criteria |
|-----------|--------|----------|
| Graph 1: Quits vs. Layoffs | 10 | Both series shown, recession shading, clear formatting |
| Part 1 Interpretation | 15 | Accurate description of patterns, correct economic reasoning |
| Graph 2: Beveridge Curve | 10 | Correct axes, color-coded by period, clear formatting |
| Part 2 Interpretation | 15 | Understands curve relationship, identifies shifts, proposes explanations |
| Policy Memo | 25 | Uses evidence, logical recommendations, professional format |
| **Total** | **75** | |

---

## Pause Point: In-Class Graph Presentation

**During Week 4 class, you will briefly present ONE of your graphs (your choice) to a small group.** You'll have 2 minutes to:
1. Show your graph
2. Explain one key finding
3. Answer one question from classmates

This is **required** - you cannot submit the final assignment without completing the presentation. Sign up for a presentation slot on [course LMS].

**Purpose:** This ensures you've engaged with the data yourself and can explain your work verbally, not just in writing.

---

## Tips for Success

1. **Start with the data** - Open the CSV file and explore it before making graphs
2. **Use specific numbers** - "The quit rate peaked at 3.0% in November 2021" is better than "quits were high"
3. **Think about mechanisms** - Don't just describe patterns; explain why they occur
4. **Keep the memo professional** - This is practice for real policy writing

---

## Resources

- JOLTS Overview: https://www.bls.gov/jlt/
- Beveridge Curve Explainer: https://www.bls.gov/opub/mlr/2010/article/the-beveridge-curve.htm
- Graph templates will be posted on [course LMS]

---

## Extra Credit (up to 10 points)

Compare JOLTS patterns in **two different industries** (e.g., leisure & hospitality vs. professional services). The full industry-level data is available at https://www.bls.gov/jlt/data.htm.

- Create one additional graph comparing quit rates by industry
- Write one paragraph explaining why the patterns differ
- What does this tell us about which workers benefited most from the tight labor market?

---

*This assignment was created for Labor Policy and the Future of Work at NYU Wagner. Data source: U.S. Bureau of Labor Statistics, Job Openings and Labor Turnover Survey.*
