# econ5200-lab11-did
Difference-in-Differences: Parallel Trends, Staggered Adoption and the Forbidden Comparison
Objective
To understand the assumptions behind difference-in-differences (DiD), identify common estimation problems, and examine how these problems affect the reliability of results.
Methodology
- Reproduced Card and Krueger's (1994) minimum-wage study using the original employment data.
- Simulated a panel with different pre-treatment trends to examine violations of the parallel trends assumption.
- Analyzed staggered treatment adoption using two-way fixed effects (TWFE) and individual 2×2 DiD comparisons.
- Compared conventional and clustered standard errors in a panel with persistent state-level shocks.
- Used AI to develop a Goodman-Bacon decomposition and tested its results against my own calculations.
Key Findings
- Card and Krueger: Reproduced an estimated employment increase of 2.75 full-time-equivalent employees, compared with the published 2.76.
- Parallel Trends: Obtained a statistically significant DiD estimate of 1.148 despite the true treatment effect being zero, demonstrating how different underlying trends can produce misleading results.
- Staggered Adoption: TWFE estimated an effect of −0.994 when the true average effect was 6.71. The comparison using already-treated units as controls accounted for 66.7% of the estimate's weight.
- Clustered Standard Errors: Conventional standard errors were approximately 8.6 times smaller than state-clustered standard errors, overstating statistical significance.
- AI Verification: Revised an AI-generated Goodman-Bacon decomposition to handle missing observations. The corrected function produced a weighted estimate of 2.6735, matching TWFE on the balanced sample.
Conclusion
This lab showed me why statistically significant DiD estimates are not necessarily reliable. Parallel trends, treatment timing, and correlated errors can all affect the results. I also learned the importance of independently checking AI-generated code before using it for statistical analysis.
