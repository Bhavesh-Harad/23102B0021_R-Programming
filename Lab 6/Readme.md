# Comprehensive Statistical Analysis of Palmer Penguins

## 1. Project Overview
This project provides an in-depth statistical analysis of the Palmer Penguins dataset to investigate variations in physical characteristics—specifically body mass and flipper length—across different species and sexes[cite: 1]. The entire analysis, including hypothesis testing and visualizations, was conducted using the R programming language[cite: 1].

## 2. Dataset Description
* **Source Package:** Built-in `palmerpenguins` R package[cite: 1].
* **Observation Pool:** Initially 344 penguins observed in the Palmer Archipelago, Antarctica[cite: 1]. After removing rows with missing values, 333 penguins were retained for analysis[cite: 1].
* **Target Species:** Adelie, Chinstrap, and Gentoo[cite: 1].

## 3. Analytical Methodology
The study employed a combination of parametric and non-parametric statistical methods to ensure robust conclusions:
* **Normality & Variance Checks:** Shapiro-Wilk tests for normality and Levene’s test for homogeneity of variance[cite: 1].
* **Two-Sample t-tests (Welch's):** Used to evaluate body mass differences between male and female groups[cite: 1].
* **Analysis of Variance (ANOVA):** One-way ANOVA for species-level trait differences, and Two-way ANOVA to evaluate the interaction between species and sex on body mass[cite: 1].
* **Post-Hoc Testing:** Tukey's Honest Significant Difference (HSD) test to identify specific pairwise differences[cite: 1].
* **Robustness Checks:** Kruskal-Wallis non-parametric tests were utilized to validate ANOVA findings against mild normality/variance assumption violations[cite: 1].
* **Effect Size:** Cohen's *d* was calculated to measure the practical significance of sex-based weight differences[cite: 1].

## 4. Detailed Findings

### A. Body Mass by Species
* Species is the dominant driver of body mass differences (One-way ANOVA: p < 2e-16)[cite: 1]. 
* Gentoo penguins are substantially heavier (mean ~5092 g) compared to both Adelie (~3706 g) and Chinstrap (~3733 g) species[cite: 1].
* Tukey HSD revealed that while Gentoo differs significantly from the other two, Adelie and Chinstrap penguins cannot be statistically distinguished from each other based on body mass alone (p = 0.916)[cite: 1].

### B. Body Mass by Sex
* Sex has a highly significant main effect on weight across all species[cite: 1]. 
* Male penguins are on average 683 g heavier than female penguins[cite: 1].
* This difference is not just statistically significant (p = 4.79e-16), but practically large, with a Cohen's *d* effect size of 0.936[cite: 1].

### C. Interaction Effects (Species × Sex)
* A Two-way ANOVA revealed a significant interaction between species and sex (p ≈ 0.0002)[cite: 1].
* This indicates that the weight gap between males and females is not uniform; specifically, the sexual dimorphism in body mass is more pronounced in the larger-bodied Gentoo penguins than in Adelie or Chinstrap penguins[cite: 1].

### D. Flipper Length Analysis
* Flipper length proved to be a more precise species discriminator than body mass[cite: 1].
* A One-way ANOVA and subsequent Tukey HSD test showed that flipper lengths differ significantly across *all three* pairwise comparisons (p < 0.001 for all)[cite: 1]. 
* Unlike body mass, flipper length successfully separates Adelie (shortest, mean ~190 mm) from Chinstrap (medium, mean ~196 mm), with Gentoo again being the largest (longest, mean ~217 mm)[cite: 1].

## 5. Conclusion
Both body mass and flipper length vary meaningfully by species and sex[cite: 1]. Gentoo penguins stand out as the largest and most physically distinct group, while male penguins consistently outweigh females across the board[cite: 1]. Flipper length serves as the most consistent metric for statistically distinguishing all three species from one another[cite: 1].
