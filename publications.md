---
title: Publications
layout: page
---

### Working Papers & Under Review

**Afari, K.B.** and Gwon, Y. (2026+) Compressed Spatio-Temporal Basis Functions: An SVD-PICAR Framework for Scalable Gaussian and Multinomial Inference. Under review at *Journal of Computational and Graphical Statistics*.
<details markdown="1"><summary>Abstract</summary>

When spatial basis representations are extended to the spatio-temporal setting, the hierarchical model dimension grows quickly due to tensor-product constructions, leading to large and redundant bases. Existing approaches such as PICAR (Projection-based Intrinsic Conditional Autoregression) improve computational efficiency by selecting a rank *r* within a user-specified maximum basis size *K* (that is, *r* ≤ *K*), but provide no principled way to choose *K* itself, leaving the selected basis potentially non-optimal for the data.

We propose ST-SVD-PICAR, which integrates randomized singular value decomposition (rSVD) into spatio-temporal (ST) basis construction. Starting from a dense tensor-product basis using mesh-based Moran eigenvectors for space and B-splines for time, rSVD removes redundant directions and extracts dominant space–time patterns in a data-driven manner. This identifies an optimal *K*, defined as the smallest basis size at which predictive accuracy is preserved, runtime stabilizes, and sampling efficiency — measured as effective sample size per second (ESS/sec) — peaks, corresponding to a computational sweet spot.

We assess candidate sizes *K* ∈ {200, 300, 400, 500, 600} under Gaussian and multinomial spatio-temporal models. Runtime stabilizes and ESS/sec peaks at *K* = 500 (Gaussian) and *K* = 400 (multinomial). Validation on two large real-world datasets shows that when *n* is substantially larger than *K*, the primary benefit shifts from computational efficiency toward prediction accuracy.

Overall, ST-SVD-PICAR provides a scalable, principled approach for high-dimensional spatio-temporal inference. Efficiency gains are most pronounced when *n* and *K* are not far apart in size, as demonstrated in the simulation studies.

</details>

**Afari, K.B.** and Gwon, Y. (2026+) SVD-PICAR Bayesian Kernel Machine Regression Framework for Spatio-Temporal Count Data. Under review at *Statistics in Medicine*.
<details markdown="1"><summary>Abstract</summary>

Bayesian kernel machine regression (BKMR) has become a widely used tool for studying the health effects of complex exposure mixtures, with extensions to overdispersed count outcomes now available. However, existing BKMR models for count data handle spatial and temporal structure separately rather than as a unified random field, leaving the joint space–time dependency in the data unmodeled. No existing method therefore combines nonlinear mixture modeling, a neighborhood-based spatio-temporal random effect, and an overdispersed count likelihood in a single computationally workable framework.

We address this gap by proposing SVD-PICAR NB-BKMR, which extends the PICAR framework from the spatial to the spatio-temporal setting through a Kronecker product of spatial and temporal bases. However, this spatio-temporal basis contains redundant components that expand the dimension of the latent random field, produce highly correlated posterior draws, and make the full-rank ICAR field ill-conditioned, weakening exposure-effect estimates and slowing MCMC sampling. We resolve this by incorporating a truncated singular value decomposition (SVD) into the spatio-temporal PICAR basis, retaining only the dominant orthogonal directions, reducing the latent field to a manageable dimension, and separating background spatio-temporal variation from the nonlinear exposure–response pattern.

We compare three competing models: a fixed effect model (M1), a full-rank mixed effect model (M2), and the proposed SVD-PICAR mixed effect model (M3). Models are evaluated through simulation and an application to county-level thyroid cancer and pesticide exposure data from Nebraska (1992–2014). In simulation, M3 achieves the best predictive fit by the Watanabe–Akaike Information Criterion (WAIC), the highest MCMC efficiency by effective sample size per second (ESS/sec), and the most stable exposure identification. In the Nebraska application, Atrazine and Alachlor emerge as the leading contributors to thyroid cancer risk, with nonlinear exposure–response relationships that remain robust after spatio-temporal correction.

The SVD-PICAR framework offers a principled and practically workable approach for mixture analysis in spatio-temporal count data settings.

</details>

Gribben, K.C., Gwon, Y., **Afari, K.**, Berman, J., Li, A., Fard, B., Abadi, A., Wardlow, B., Tong, D., Tao, Z., and Bell, J. (2026+) Drought increases the risk of COPD mortality in the United States. Under review at *Environmental Research*.
<details markdown="1"><summary>Abstract</summary>

Chronic obstructive pulmonary disease (COPD) is a leading cause of death and disability in the United States (U.S.). Drought is connected to multiple environmental risk factors for COPD mortality, but prior studies have not examined associations between drought indicators and COPD mortality in the United States at national and regional levels.

We conducted an ecological study at national and regional levels during 2003-2021 for the contiguous U.S. Monthly drought was defined according to the United States Drought Monitor (USDM) and Gravity Recovery and Climate Experiment (GRACE) surface soil moisture anomalies analyzed as tertiary (none, moderate, severe) and binary (drought, no drought) variables. COPD mortality data were obtained from the CDC National Center for Health Statistics. Two-stage quasi-Poisson regression models were fit and adjusted for county annual smoking prevalence, monthly temperature and time trends.

Nationwide severe drought conditions characterized by GRACE were associated with a 2% increased risk of COPD mortality. Regionally, USDM and GRACE severe drought increased the risk of COPD mortality in the Upper Midwest by 6% and 7%, respectively. GRACE tertiary drought was also associated with COPD mortality in the Northwest (increase 3-4%) and Northern Rockies and Plains (increase 5-10%). Tertiary USDM drought was associated with reduced risk of COPD mortality in the West.

COPD mortality was greater during drought conditions in the contiguous United States. Drought’s impact on COPD mortality varies by region, drought metric and severity. Future research may examine environmental mediators or compounding exposures to better understand how drought leads to increased morbidity and mortality among COPD populations.

</details>


**Afari, K.B.** et al (2026+) A Cluster-Based Framework for Joint Mixture Effects: Extending SVD-PICAR Bayesian Kernel Machine Regression to Spatio-Temporal Count Outcomes ( In preparation for Biometrics )


**Afari, K.B.** (2026+) stsvdpicar: An R Package for Scalable Bayesian Spatio-Temporal Inference via SVD-PICAR. Software paper in preparation for the Journal of Statistical Software. Repository: [GitHub URL once available]

### Published

**Afari, K.B.** and Lewis, C.N.H. (2022) Performance Comparison of Imputation Methods for Mixed Data Missing at Random with Small and Large Sample Dataset with Different Variability. *Asian Journal of Probability and Statistics*, **20**(2), 16--39. [`https://journalajpas.com/index.php/AJPAS/article/view/416`](https://journalajpas.com/index.php/AJPAS/article/view/416){:target="_blank" rel="noopener"}

**Afari, K.B.** (2022) The role of fixed income in pension scheme investment in Ghana: A possible adoption for the United States economy. *Research Journal of Finance and Accounting*, **13**(14), 27--35. [`https://iiste.org/Journals/index.php/RJFA/article/view/59308/61231`](https://iiste.org/Journals/index.php/RJFA/article/view/59308/61231){:target="_blank" rel="noopener"}
