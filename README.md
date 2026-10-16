# Paradox of Choice in Retail Selection

**Between-subjects experiment on how assortment size affects decision time, purchase behavior, and post-choice emotions** — designed in Qualtrics, analyzed in R.

[View the live analysis report](https://quudus.github.io/paradox-of-choice-portfolio)

## What the experiment tested

Does having more choices actually make decisions harder? 74 participants were randomly assigned to one of two conditions:

- **4-option group** — chose from a small product assortment
- **16-option group** — chose from a larger product assortment

After deciding, participants answered questions on satisfaction, confidence, and regret.

## What was measured

| Variable | What it captures |
|---|---|
| Decision Time (seconds) | How long the participant spent on the choice page before submitting |
| Purchase | Whether they selected a product (1) or walked away (0) |
| Satisfaction (1–5) | How satisfied they were with their experience |
| Confidence (1–5) | How confident they felt in their decision |
| Regret (1–5, purchasers only) | Whether they felt another option might have been better |

## Key findings

- **The 16-option group took nearly twice as long to decide** — 19.5 sec vs. 10.2 sec on average (Welch t-test: t≈4.80, p<.001). More choices clearly slowed people down.
- **Purchase behavior did not differ significantly** between the two groups — having 16 options didn't stop people from buying.
- **No significant difference in satisfaction, confidence, or regret** — post-choice emotions were similar regardless of how many options were available.

## Statistical tests run

5 tests in R across the outcome variables:

- Welch t-test (decision time)
- Mann-Whitney U test (decision time, non-parametric check)
- Two-proportion z-test (purchase rate)
- ANOVA (satisfaction, confidence, regret)

## Tools and workflow

- **Qualtrics** — survey design, Randomizer block for automated random assignment
- **Excel** — data cleaning using the 1.5×IQR method to remove outliers
- **R** — statistical analysis and report generation (R Markdown)
- Data: 74 participants collected; 71 retained after outlier removal

## Files in this repo

| File | What it is |
|---|---|
| `index.html` | Full analysis report (rendered from R Markdown) |

Raw data and the .Rmd source are available on request.
