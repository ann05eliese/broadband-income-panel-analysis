# Broadband Internet Access and Household Median Income: A Panel Data Analysis

**Author:** Anneliese Hall  
**Methodology:** Panel Data Fixed Effects Regression ($R$)  
**Data Source:** U.S. Census Bureau ACS 5-Year Estimates (2017 & 2022)

---

## Summary
This study investigates the relationship between broadband internet access and median household income across all 46 counties in South Carolina. Utilizing a panel data analysis with county and time fixed effects, the research tests whether increased broadband infrastructure correlates with income growth, specifically comparing rural vs. urban dynamics. 

### Key Findings:
* **Positive Correlation:** Across all models, broadband internet access exhibits a positive relationship with median household income for both urban and rural counties.
* **Marginal Effects:** Fixed effects models indicate that rural counties experience a slightly higher marginal income benefit per 1% increase in broadband infrastructure than urban counties, though the difference is statistically non-significant ($p = 0.343$).
* **Hierarchical Diffusion:** Visually, within-county demeaned data illustrates a distinct clustering among urban counties, highlighting a synchronous adoption pattern and a structural lag in rural infrastructure adaptation.

---

## Econometric Framework
To account for unobserved time-invariant heterogeneity across South Carolina's diverse counties, the primary model implements a log-log fixed effects specification:

$$\log(\text{median income}_{it}) = \beta_1 \log(\text{broadband \%}_{it}) \times \text{county type}_{it} + \beta_2 \log(\text{total pop}_{it}) + \alpha_i + \delta_t + \varepsilon_{it}$$

Where:
* $\alpha_i$ represents **County Fixed Effects** (permanent differences in wealth and regional industries).
* $\delta_t$ represents **Time Fixed Effects** (broader macro trends affecting the whole state between 2017 and 2022).
* $$\log(\text{total pop})$$ controls for **agglomeration effects** (larger populations generating higher incomes naturally).

---

## Theoretical Background & Literature
* **Everett M. Rogers (Diffusion of Innovations):** Applies the theory of hierarchical diffusion to explain how urban epicenters adopt infrastructure innovations rapidly, leaving a structural adoption lag in rural communities. 
* **Röller & Waverman / Czernich et al.:** Explores the reduction of transaction and information search costs resulting from high-speed communications, shifting the localized production function upward.
