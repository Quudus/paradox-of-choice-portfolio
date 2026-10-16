# Paradox of Choice in Retail Selection

**Decision Time, Purchase Behavior, and Post-Choice Emotions** — a between-subjects experiment designed in Qualtrics and analyzed in R across 71 participants.

[View the live analysis report](https://quudus.github.io/paradox-of-choice-portfolio)

## What the experiment tested

Two groups, one question — does having more choices make decisions harder?

| Group | Condition |
|---|---|
| 4-option group | Chose from a small product assortment |
| 16-option group | Chose from a larger product assortment |

After deciding, participants rated their satisfaction, confidence, and regret.

## Key findings

- **The 16-option group took nearly twice as long to decide** — 19.5 sec vs. 10.2 sec on average (Welch t-test: t≈4.80, p<.001). More choices clearly slowed people down.
- **Purchase behavior did not differ significantly** between the two groups — having 16 options didn't stop people from buying.
- **No significant difference in satisfaction, confidence, or regret** — post-choice emotions were similar regardless of how many options were available.

## Tools used

- **Qualtrics** — survey design and Randomizer block for automated random assignment
- **Excel** — data cleaning using the 1.5×IQR method to remove outliers
- **R** — 5 statistical tests (Welch t-test, Mann-Whitney U, two-proportion z-test, ANOVA) and report generation

## Files in this repo

| File | What it is |
|---|---|
| `index.html` | Full analysis report rendered from R Markdown |

The interactive report is published on GitHub Pages — see the link above.
