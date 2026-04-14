# Traumatic Brain Injury Longitudinal Analysis

This project studies whether traumatic brain injury (TBI) is associated with ongoing structural brain degeneration over time. The main outcome variable is left hippocampus total volume (HPC_L_TOT), a brain region closely related to memory and cognitive functioning. The analysis also examines whether cognitive therapy is linked to slower decline and whether preserved brain structure corresponds to better cognitive quality of life. 

## Project questions

1. Do individuals with TBI show faster decline in left hippocampal volume over time than healthy controls?
2. Within the TBI group, is cognitive therapy associated with a slower rate of structural decline?
3. Is preserved hippocampal volume associated with better cognitive quality-of-life scores?

## Data

The dataset contains repeated brain measurements for injured patients and healthy controls. The data were converted from wide form to long form for longitudinal analysis. Key variables include:

- `HPC_L_TOT` = Left hippocampus total volume
- `VBR` = Ventricle-to-brain ratio
- `tothrsCOG` = Total hours of cognitive therapy
- `LAQ_cogtot` = Cognitive quality-of-life score

The final analysis dataset includes subject ID, time in years, hippocampal volume, group, age, sex, VBR, therapy hours, and cognitive outcome score. :contentReference[oaicite:1]{index=1} :contentReference[oaicite:2]{index=2}

## Methods

The main method used in this project is the linear mixed-effects model, which is appropriate for repeated measurements from the same individuals over time. The models include random intercepts and random slopes to account for subject-level variation. The analysis also adjusts for age and sex as confounders. :contentReference[oaicite:3]{index=3}

## Main findings

- TBI patients showed significantly faster decline in left hippocampal volume over time than healthy controls.
- The interaction term suggested that injured patients lose about 65 mm³ more hippocampal volume per year compared with controls.
- Cognitive therapy showed a slight positive trend, but there was no strong statistical evidence that more therapy hours slowed structural decline.
- Preserved hippocampal volume was not significantly associated with better cognitive quality-of-life scores.
- Hippocampal decline was negatively correlated with ventricular expansion, supporting the interpretation of real structural degeneration. :contentReference[oaicite:4]{index=4} :contentReference[oaicite:5]{index=5} :contentReference[oaicite:6]{index=6} :contentReference[oaicite:7]{index=7}

## Files

- `final report.pdf` — full written report
- `tbi kixed models analysis.Rmd` — R Markdown code
- `TBI.xlsx` — dataset

## Tools used

- R
- R Markdown
- Linear mixed-effects models
- Longitudinal data analysis

## Conclusion

This project suggests that traumatic brain injury may be associated with long-term structural brain degeneration rather than a one-time event. It also shows that structural preservation alone may not fully explain functional recovery, which may depend on broader recovery mechanisms. :contentReference[oaicite:8]{index=8}
