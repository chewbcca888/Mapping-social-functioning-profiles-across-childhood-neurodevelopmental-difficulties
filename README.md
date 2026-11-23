# Mapping social functioning profiles across childhood neurodevelopmental difficulties

Code accompanying:

Trachtenberg, E., Mousley, A., Jelen, M., & Astle, D. *Mapping social functioning profiles across childhood neurodevelopmental difficulties: links with diagnosis, cognition, and everyday executive function.*

## Files

The files follow the order of the analysis pipeline (Figure 1 in the paper):

| File | Language | Description |
| --- | --- | --- |
| `01_network_analysis.Rmd` | R | Regularised partial correlation network (EBICglasso) of 22 parent-report social items (SDQ, CCC-2, Conners-3) and Louvain community detection, used to derive the four social dimensions |
| `02_SOM_social_profiles.ipynb` | Python | Self-organising map of the four social dimensions, simulated archetypes, one-vs-rest SVM classification, permutation-based island-size test, profile membership and centroid-distance scores |
| `03_GAM_age.Rmd` | R | Generalised additive models of age and profile expression (centroid-distance scores) and of the social dimension scores, adjusted for sex and referral status |

## Data availability

No data are included in this repository; the code is shared to show the analysis. Data from the Centre for Attention, Learning and Memory (CALM) are available via the [CALM data portal](https://portal.camide.cam.ac.uk/overview/1158), subject to the cohort's data access procedures.

## Software

Python (v3.11.13): numpy, pandas, MiniSom, scikit-learn, scipy, statsmodels, matplotlib, seaborn.
R (v4.3.3): tidyverse, polycor, corrplot, qgraph, igraph, mgcv.

## Contact

Estherina Trachtenberg, et581@cam.ac.uk, University of Cambridge.
