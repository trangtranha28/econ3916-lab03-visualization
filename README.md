# Honest vs. Misleading Visualizations

## Objective
Demonstrate, using synthetic and real economic data, how chart design and skipped exploratory analysis can distort quantitative evidence, and build practical tools for producing and auditing honest visualizations.

## Methodology
- **Anscombe's Quartet:** Recreated the four datasets, which share nearly identical means (x ≈ 9, y ≈ 7.5), variances, and correlation (r ≈ 0.82) but have very different underlying shapes, and plotted them side by side.
- **Lie Factor audit:** Computed a Lie Factor of **[YOUR VALUE]** for a truncated-axis revenue chart (the ratio of the effect shown in the graphic to the effect in the data), then redesigned the chart with a zero-based axis and proportional encoding.
- **Framing experiment:** Pulled average hourly earnings from FRED (series AHETPI), deflated to 2020 dollars, and produced four visualizations of the same real series that supported four different narratives through choices of axis range, baseline, time window, and nominal vs. real values.
- **Structured EDA checklist:** Applied a four-step workflow (structure, distributions, relationships, anomalies) to World Bank GDP data covering **[YOUR VALUE]** countries over **[YOUR VALUE]** years.
- **Interactive tool:** Built a toggle that switches between misleading and honest chart designs and recalculates the Lie Factor live.

## Key Findings
- Summary statistics alone can hide fundamental differences in data. Anscombe's Quartet shows identical numerical summaries across datasets that are linear, curved, outlier-driven, or leverage-driven.
- A truncated axis produced a Lie Factor of **[YOUR VALUE]**. Values well above 1 indicate visual exaggeration, while honest charts stay close to 1.
- The same inflation-adjusted earnings series can be made to look like growth, stagnation, or decline through design choices alone, so chart framing is an analytical decision with consequences.
- Systematic EDA of the GDP data surfaced [YOUR FINDING, e.g., skewed distributions, missing values, or outlier economies] before any modeling or plotting.
- Quantifying distortion with a live metric makes chart integrity measurable and easier to teach and review.
