# Growth and Characterization of Magnetoelectric Thin Films by Pulsed Laser Deposition

**Project type:** Thin-film deposition and materials characterization  
**Material system:** Barium titanate (BTO) and cobalt ferrite (CFO)  
**Deposition method:** Pulsed Laser Deposition (PLD)  
**Laser source:** KrF excimer laser, approximately 248 nm  
**Substrate stack stated in the project presentation:** Pt/Ti/SiO₂/Si  
**Seed layer:** LSCO (lanthanum strontium cobalt oxide)

## Project overview

This repository documents an internship project on the growth and characterization of BTO–CFO magnetoelectric thin-film structures using pulsed laser deposition. The accompanying presentation identifies BTO and CFO powders synthesized through a solid-state route, pelletization, substrate preparation, LSCO seed-layer deposition, and subsequent PLD thin-film deposition.

The project explores structural and vibrational characterization through X-ray diffraction (XRD), cross-sectional scanning electron microscopy (SEM), and Raman spectroscopy. The presentation includes XRD patterns for BTO/CFO/LSCO/Pt/Ti/SiO₂/Si and CFO/BTO/LSCO/Pt/Ti/SiO₂/Si structures.

## Objectives

- Document the fabrication workflow for BTO–CFO thin-film structures by PLD.
- Organize the XRD reflection assignments reported in the presentation.
- Present the available XRD and Raman figures with their original context.
- Outline how SEM and Raman characterization complement structural analysis.
- Identify which conclusions can be drawn from the presentation and which require raw data or additional measurements.

## Experimental workflow documented in the presentation

1. Synthesis of BTO and CFO powders using a solid-state route.
2. Target preparation by pelletization.
3. Substrate preparation using a Pt/Ti/SiO₂/Si stack.
4. LSCO seed-layer deposition.
5. Thin-film deposition by PLD using a KrF excimer laser (approximately 248 nm).
6. Characterization using XRD, cross-sectional SEM, and Raman spectroscopy.

The presentation does not provide complete numerical process settings such as laser fluence, repetition rate, substrate temperature, oxygen pressure, target-to-substrate distance, or deposition duration. These are intentionally not inferred here.

## XRD observations reported

The presentation assigns the following reflections:
- BTO: (110), (111), and (200), described in the presentation as indicating tetragonal BTO.
- CFO: (220), (311), and (400), described in the presentation as indicating cubic spinel CFO.

Additional labels are visible in the plotted patterns. The complete raw intensity-versus-2θ data and reference-card details were not supplied, so this repository does not independently re-index the patterns or claim a new phase verification.

See:
- `figures/xrd_bto_cfo_bto_cfo.png`
- `figures/xrd_cfo_bto_bto_cfo.png`

## Raman and SEM characterization

The presentation includes Raman spectra for BTO/CFO and CFO/BTO thin-film structures and a cross-sectional SEM image with layer labels. The original numerical Raman data and SEM image measurements are not provided as separate data files. Accordingly, the figures are included for documentation, not for quantitative re-analysis.

See `figures/raman_spectra.png`.

## Repository contents

- `data/xrd_reflection_assignments.csv` — reflection labels and phase assignments transcribed from the presentation.
- `notebooks/project_data_exploration.ipynb` — a reproducible notebook that loads and summarizes the documented reflection assignments.
- `figures/` — figures extracted from the presentation.
- `docs/methodology_and_limitations.md` — workflow, evidence boundaries, and possible next steps.

## Reproducibility

The notebook uses Python, pandas, and Matplotlib. Install dependencies with:

```bash
pip install -r requirements.txt
```

Open `notebooks/project_data_exploration.ipynb` in Jupyter Notebook or Google Colab and run the cells in order.

## Limitations and next steps

This repository is based on a project presentation, not the complete experimental record. It does not contain raw XRD counts, numerical Raman spectra, raw SEM image files, dielectric measurement tables, or complete PLD process logs. Quantitative analysis such as peak fitting, lattice-parameter calculation, crystallite-size estimation, Raman peak fitting, layer-thickness uncertainty, and dielectric-property comparison should be performed only when the corresponding raw data and measurement details are available.

Potential future additions:
- Raw XRD data (2θ and intensity) and reference patterns.
- Raw Raman shift and intensity data.
- SEM micrographs with scale bars and documented layer-thickness measurements.
- Dielectric measurement data and frequency/measurement conditions.
- Full PLD process parameters and a comparison of BTO/CFO versus CFO/BTO layer sequences.

## Acknowledgment

The source presentation identifies Prof. Ajit R. Kulkarni as the project guide. Please ensure you have permission to publish any institutional, laboratory, or unpublished research material before making this repository public.
