# Nigeria Brucellosis GIS & Surveillance Analysis (2008–2025)

## Overview

This project examines the geographical distribution, temporal reporting patterns, *Brucella* species classifications and animal-host profiles of reported animal brucellosis in Nigeria from 2008 to 2025, using data extracted from the World Organisation for Animal Health's World Animal Health Information System (WOAH-WAHIS).

The analysis combines descriptive epidemiology, geographical visualisation and spatial autocorrelation methods to investigate patterns in reported cases and outbreaks. It adopts a One Health surveillance perspective, recognising the importance of animal health surveillance to integrated approaches to zoonotic disease monitoring.

**Important:** The findings describe reported surveillance records, not the true incidence or prevalence of brucellosis in Nigeria.

## Research questions

1. How were reported brucellosis cases and outbreaks distributed across Nigeria's first-level administrative units between 2008 and 2025?
2. How did annual reporting patterns and the geographical breadth of reporting change over time?
3. Which *Brucella* species classifications and animal hosts accounted for the reported records?
4. Was there evidence of global or local spatial autocorrelation in reported cases and outbreaks?
5. What do the observed patterns and data limitations imply for animal disease surveillance and One Health coordination?

## Key findings

- **487 reported cases** and **78 reported outbreaks** were identified in the extracted records.
- Reports were recorded in **20 of 37 first-level administrative units** (36 states and the Federal Capital Territory).
- *Brucella abortus* accounted for **417 reported cases (85.6%)**.
- Cattle accounted for **281 cases (57.7%)**, while swine accounted for 95 (19.5%).
- Global spatial autocorrelation for reported case counts was not statistically significant (Moran's I = −0.0504; pseudo-p = 0.409).
- Reported outbreak counts showed weak positive global spatial autocorrelation (Moran's I = 0.1662; pseudo-p approximately 0.04), with sensitivity to permutation seeds.
- Reporting breadth increased in 2021–2025. This may reflect changes in reporting visibility and surveillance processes; the analysis cannot establish that disease occurrence increased.

## Analytical approach

The project covers:

- Data organisation and descriptive epidemiology.
- Annual trends in reported cases, outbreaks and reporting breadth.
- Geographic comparison of administrative units.
- *Brucella* species and animal-host distributions.
- Global Moran's I using Queen-contiguity spatial weights.
- Local Moran's I (LISA) for exploratory identification of spatial patterns.
- Sensitivity checks and interpretation of statistical uncertainty.
- One Health implications and surveillance recommendations.

Spatial analyses used row-standardised Queen-contiguity weights and 999 conditional permutations. Local spatial findings are interpreted cautiously because of sensitivity to permutation results and multiple testing.

## Selected spatial findings

For reported outbreak counts, Kaduna showed a high–high local association, Katsina a low–high association, and Rivers a low–low association under the exploratory local analysis. These results should not be interpreted as definitive evidence of transmission pathways or disease-risk hotspots. None remained significant after Bonferroni correction for 37 local tests.

No robust local spatial association was identified for reported case counts.

## One Health relevance

The results illustrate how animal disease reporting data can support geographical surveillance review, identify gaps in reporting visibility and guide questions for further investigation. They also highlight the importance of improving species identification, host information, diagnostic documentation and linkage between animal and human health surveillance.

The analysis does not include linked human or environmental surveillance data and therefore does not directly measure cross-sector transmission.

## Data source and reproducibility

**Primary source:** World Organisation for Animal Health (WOAH), World Animal Health Information System (WAHIS).

The repository will document the extraction period, data preparation, variable definitions, analytical workflow, software and references as these are verified against the original files.

The extracted dataset contains reporting limitations, including records without event identifiers and incomplete diagnostic fields. Raw data will only be redistributed if the applicable access and reuse conditions permit it. Otherwise, the repository will provide appropriate documentation, code and derived outputs that can be shared responsibly.

## Limitations

- Reported counts are not population-adjusted incidence or prevalence estimates.
- Units without reports must not be considered disease-free.
- Reporting completeness and surveillance intensity may vary by place and time.
- Some records lack identifiers needed for deduplication.
- Host, diagnostic and outbreak fields are incomplete in some records.
- Species classifications are retained as reported; they are not independently laboratory-validated by this analysis.
- Local spatial findings are exploratory and subject to multiple-testing limitations.
- The analysis cannot establish causality, transmission routes or human infection risk.

## Repository structure

- `figures/` — maps and analytical visualisations.
- `data/` — data access and dictionary documentation.
- `analysis/` — descriptive analysis and reproducible workflow.
- `spatial-analysis/` — spatial weights, global Moran's I and LISA documentation.
- `tables/` — derived summary tables.
- `references/` — source and methodological references.

## Author and purpose

Developed as a public-health and One Health surveillance research portfolio project, with an emphasis on epidemiological interpretation, GIS, reproducibility and evidence-informed programme planning.

This is an independent analytical project and does not represent an official WOAH assessment or an endorsement by WOAH.
