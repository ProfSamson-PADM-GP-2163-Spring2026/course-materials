# Assignment 4: Minimum Wage Policy Analysis

**Course:** Labor Policy and the Future of Work
**Connects to:** Week 6 - Minimum Wage Policy
**Due Date:** [To be determined]
**Points:** 75

---

## Overview

The minimum wage is one of the most debated labor policies. Economic theory predicts that a higher minimum wage should reduce employment (if the labor market is competitive) or have little effect (if employers have market power). This assignment examines real-world evidence using a "natural experiment" - comparing employment in neighboring counties with different minimum wage policies.

**Data is provided** - you will focus on analysis and interpretation, not data collection.

---

## Learning Objectives

By completing this assignment, you will:

1. Understand how minimum wage policies vary across states and over time
2. Apply the difference-in-differences method to estimate policy effects
3. Critically evaluate causal claims from observational data
4. Weigh competing economic models (competitive vs. monopsony)
5. Form evidence-based policy positions while acknowledging uncertainty

---

## Background: The Minimum Wage Debate

**The Competitive Model Prediction:**
- Minimum wage = price floor above equilibrium
- Employers hire fewer workers → employment falls
- Workers who keep jobs benefit; those who lose jobs are harmed

**The Monopsony Model Prediction:**
- Employers have wage-setting power (not many competing employers)
- They pay workers less than their productivity
- Minimum wage can raise wages WITHOUT reducing employment (up to a point)

**Empirical Evidence:**
- Classic Card & Krueger (1994): Found NO employment effect from NJ minimum wage increase
- Recent studies: Mixed results, but generally find small or zero employment effects
- Possible explanations: Monopsony power, reduced turnover costs, productivity gains, price pass-through

---

## The Data

Download from [course LMS]: **`minimum_wage_border_counties.csv`**

This dataset covers **selected border county pairs** from 2010-2019 (before COVID):

| Variable | Description |
|----------|-------------|
| `county_fips` | County identifier |
| `county_name` | County name |
| `state` | State |
| `year` | Year |
| `min_wage` | Effective minimum wage (higher of state or federal) |
| `emp_food_service` | Employment in food services (NAICS 722) |
| `emp_retail` | Employment in retail trade |
| `avg_wage_food` | Average weekly wage in food services |
| `pair_id` | Border pair identifier (counties in same pair share a border) |
| `treatment` | 1 if state raised minimum wage above federal, 0 otherwise |

**The border county pairs are:**

| Pair | High-Wage County | Low-Wage County | Wage Difference (2019) |
|------|------------------|-----------------|------------------------|
| 1 | King County, WA (Seattle) | Kootenai County, ID | ~$5.50 |
| 2 | Marin County, CA | Douglas County, NV | ~$4.00 |
| 3 | Philadelphia County, PA | Gloucester County, NJ* | ~$3.00 |

*Note: NJ has since raised its wage above PA, but during our sample period, PA was often higher for Philadelphia specifically.

---

## Part 1: Descriptive Analysis (20 points)

### Task 1.1: Map the Variation

Using the data provided (or looking up states online), create a **simple table or map** showing:
- States with minimum wage = federal ($7.25) as of 2019
- States with minimum wage between $8-$11
- States with minimum wage above $11

You can create a simple table categorizing states, or use any mapping tool you're comfortable with.

**Deliverable:** Table or map showing minimum wage variation

### Task 1.2: Summary Statistics

Using the provided data, create a **summary table** comparing treated vs. control counties:

| Statistic | High-Wage Counties | Low-Wage Counties |
|-----------|-------------------|-------------------|
| Average minimum wage (2019) | | |
| Average food service employment (2019) | | |
| Average weekly wage, food services (2019) | | |
| Number of counties | | |

### Task 1.3: Interpretation (Half page)

- Do high-wage and low-wage counties look similar in terms of employment levels?
- Are there any obvious differences that might concern you for making comparisons?
- Why might comparing border counties be better than comparing random counties across the country?

---

## Part 2: Difference-in-Differences Analysis (30 points)

### The Method

**Difference-in-differences (DiD)** compares:
1. Change over time in treated units (counties that raised minimum wage)
2. Change over time in control units (counties that didn't)

The difference between these changes is our estimate of the policy effect.

```
DiD = (Treated_After - Treated_Before) - (Control_After - Control_Before)
```

### Task 2.1: Visual Analysis

For **Border Pair 1** (King County, WA vs. Kootenai County, ID), create a **line graph** showing:
- X-axis: Year (2010-2019)
- Y-axis: Employment in food services
- Two lines: one for each county
- Mark the year(s) when Washington raised its minimum wage significantly

**Deliverable:** Time series graph for Pair 1

### Task 2.2: Calculate the DiD Estimate

Using the data, calculate the difference-in-differences for **food service employment** in Pair 1:

**Step 1:** Calculate the "before" period average (2010-2013) for each county
**Step 2:** Calculate the "after" period average (2016-2019) for each county
**Step 3:** Calculate the change for each county
**Step 4:** Calculate the difference in changes

Fill in this table:

| County | Before (2010-2013 avg) | After (2016-2019 avg) | Change |
|--------|------------------------|----------------------|--------|
| King County, WA (treated) | | | |
| Kootenai County, ID (control) | | | |
| **Difference-in-Differences** | | | |

**Express your DiD estimate as a percentage change:**
- If King County employment was 50,000 and DiD = -500, that's -1%

### Task 2.3: Interpretation (1 page)

Answer the following questions:

**A.** What is your estimated effect of the minimum wage increase on food service employment? Is it positive, negative, or close to zero?

**B.** Does this support the competitive model (employment falls) or the monopsony model (employment unchanged or rises)?

**C.** The key assumption of DiD is "parallel trends" - that treated and control counties would have had the same employment trend in the absence of treatment. Looking at your graph, do the two counties have similar trends BEFORE the minimum wage increase? If not, how does this affect your confidence in the results?

**D.** Name two other factors (besides minimum wage) that might have affected Seattle-area employment differently than northern Idaho. How might these confound your estimate?

---

## Part 3: Policy Position Paper (25 points)

Write a **2-page position paper** arguing for OR against a federal minimum wage increase to $15/hour.

### Requirements

**1. State your position clearly** (1 paragraph)
- Support, oppose, or support with modifications

**2. Summarize the evidence** (1 page)
- What does your analysis suggest about employment effects?
- What do other studies find? (cite at least one study from class)
- How confident should we be in these findings?

**3. Consider both sides** (half page)
- What's the strongest argument for the OTHER side?
- How would you respond to that argument?

**4. Acknowledge limitations** (1 paragraph)
- What don't we know?
- What additional evidence would help you be more confident?

### Grading Notes

You will be graded on the quality of your argument, not on which position you take. Strong papers:
- Use evidence appropriately (don't overstate what the data shows)
- Acknowledge uncertainty
- Engage with counterarguments
- Are clearly written

---

## Submission Requirements

Submit via [course LMS]:

1. **Part 1:** Minimum wage map/table, summary table, interpretation
2. **Part 2:** Time series graph, DiD calculation table, interpretation
3. **Part 3:** Position paper (2 pages)

**Total length:** Approximately 5-6 pages plus graphs/tables

**File naming:** `LastName_FirstName_Assignment4.pdf`

---

## Grading Rubric

| Component | Points | Criteria |
|-----------|--------|----------|
| Part 1: Descriptive analysis | 20 | Accurate summary statistics, reasonable interpretation |
| Part 2: Graph | 10 | Clear visualization, correctly labeled |
| Part 2: DiD calculation | 10 | Correct arithmetic, proper interpretation |
| Part 2: Interpretation | 10 | Understands parallel trends, identifies confounds |
| Part 3: Position paper | 25 | Evidence-based, acknowledges uncertainty, engages counterarguments |
| **Total** | **75** | |

---

## Staged Submission (Pause Point)

This assignment has a **required midpoint check-in:**

**By [date TBD]:** Submit your Part 1 (descriptive analysis) and Part 2 graph via [course LMS].

I will provide brief feedback before you complete the DiD calculations and position paper. This ensures you're on the right track with the data.

---

## Tips for Success

1. **Don't overstate your findings** - One border pair comparison is suggestive, not definitive
2. **Percentage changes are more meaningful than levels** - A 500-job change means different things for a county with 10,000 vs. 100,000 jobs
3. **Think about mechanisms** - If you find small effects, WHY might that be?
4. **Anticipate objections** - A strong argument addresses the best counterarguments

---

## Resources

- Card & Krueger (1994) "Minimum Wages and Employment: A Case Study of the Fast-Food Industry"
- Dube, Lester & Reich (2010) "Minimum Wage Effects Across State Borders"
- CBO (2019) "The Effects on Employment and Family Income of Increasing the Federal Minimum Wage"
- Course textbook chapter on minimum wage

---

## Discussion Questions (For Class)

Be prepared to discuss:

1. If minimum wage increases don't reduce employment, why do many economists still worry about very high minimums ($20+)?

2. Even if employment doesn't fall, could minimum wage increases have OTHER effects? (Hours, benefits, prices, automation)

3. Should the federal minimum be the same everywhere, or vary by local cost of living?

4. Seattle raised its minimum to $15+ and didn't see obvious job losses. Can we generalize from Seattle to rural areas?

---

*This assignment was created for Labor Policy and the Future of Work at NYU Wagner. Data sources: BLS Quarterly Census of Employment and Wages, UC Berkeley Labor Center.*
