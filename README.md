# Bed Topography of the Rutford Ice Stream
Authors: Laila Zaidi, Dr. Emma (Mickey) MacKie, Niya Shao

This repository contains the full workflow for generating stochastic realizations of Rutford Ice Stream's bed topography and ice thickness through a new approach that uses geostatistical methods, particularly the Markov chain Monte Carlo (MCMC).

This study is focused on the Rutford Ice Stream, located in West Antarctica, which flows rapidly between the Ellsworth Mountains and the Fletcher Promontory and into the Ronne Ice Shelf. Its fast flow speed, deep basal trough, and sensitivity to upstream and downstream forcing make it an ideal study site for exploring uncertainty in subglacial conditions.

---

## Study Area
The Rutford Ice Stream is one of the most powerful ice streams on the continent, flowing ~1 km/year. Its deeply eroded trough, constrained by narrow mountain walls, makes its subglacial topography both difficult to measure and essential for ice-dynamic modeling (Doake et al.).

---

## Project Overview

Glacier bed topography strongly controls ice flow, grounding-line stability, and mass balance. However, direct measurements of the bed are sparse, so we need interpolation methods that are both realistic and physically consistent. In this project, we aimed to:

 - Estimate uncertain subglacial topography for Rutford Ice Stream

 - Generate multiple stochastic realizations using MCMC sampling

 - Analyze the uncertainty in the reconstructed bed

 - Provide a reproducible workflow for future glaciology research  

### (Placeholder Images):
- Map of Rutford Ice Stream surface velocity (m/yr)
- Velocity vectors overlaid
- Grounding line shown in black
- Study domain outlined
Status: still an early draft, placeholders for data and figures.

---

## 2. Environment

We recommend creating a conda (or R) environment with the necessary packages.  
For example:  
conda env create -f environment.yml
conda activate rutford_env

---

## 3. Usage

Step by step on how to reproduce the results. 

---

## 4. Data + Methods 

Placeholders and Images:
The data section includes surface velocity, ice surface elevations, bed elevation, ice thickness, etc. 

Placeholders and Images: 
 - Sequential Gaussian Simulation (SGS): Use a variogram model derived from the radar data to generate stochastic bed realizations and preserve realistic small-scale roughness in bed elevation.

 - Mass-Conserving Adjustment (MCMC): Use Monte Carlo Markov Chains to adjust the SGS realizations and minimize a mass flux residual between modeled and observed ice flux.

 - Evaluation: Compare the final bed to the initial product using:
   - Variograms (for roughness)
   - Maps of mass flux residual
   - Visual comparison of cross-sections.

---

  ## 5. Results: 

  Placeholder Images: 
  - Variogram Comparison
  - Bed Elevation Maps
  - Mass Flux Residuals

---

## 6. References:

Doake, C.S.M., et al. “Rutford Ice Stream, Antarctica - British Antarctic Survey.” British Antarctic Survey, Aug. 2025, www.bas.ac.uk/data/our-data/publication/rutford-ice-stream-antarctica/.
