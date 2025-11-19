# Bed Topography of the Rutford Ice Stream
Authors: Laila Zaidi, Emma (Mickey) MacKie, Niya Shao

Description: this repository contains code and draft figures for estimating the bed topography beneath Rutford Ice Stream using mass-conserving interpolation methods. The current version is a work in progress with placeholder figures and partially complete analysis.

---

## 1. Overview

Glacier bed topography strongly controls ice flow, grounding-line stability, and mass balance. However, direct measurements of the bed are sparse, so we need interpolation methods that are both realistic and physically consistent.

Write ~2-3 paragraphs explaining:

Why bed topography matters for ice streams / glaciers.

Why you chose Rutford Ice Stream.

What gap you are addressing (e.g., lack of data, need for mass-conserving interpolation).

Study Area: Rutford Ice Stream

Rutford Ice Stream is a fast-flowing ice stream in West Antarctica that drains into the Ronne Ice Shelf. It is known for high ice velocities and complex basal conditions.

- **Region:** West Antarctica  
- **Feature type:** Fast-flowing outlet / ice stream  

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

Placeholders: 
The data section includes surface velocity, ice surface elevations, bed elevation, ice thickness, etc. 

Placeholders: 
Preprocess data: reproject all datasets to a common polar stereographic CRS.

Clip to the Rutford study region and create a regular grid.

Initial bed estimate

Start from an existing bed product or simple interpolation of radar picks.

Sequential Gaussian Simulation (SGS)

Use a variogram model derived from the radar data to generate stochastic bed realizations.

Preserve realistic small-scale roughness in bed elevation.

Mass-Conserving Adjustment (MCMC)

Use Monte Carlo Markov Chains to adjust the SGS realizations.

Minimize a mass flux residual between modeled and observed ice flux.

Evaluation

Compare the final bed to the initial product using:

Variograms (for roughness)

Maps of mass flux residual

Visual comparison of cross-sections.
