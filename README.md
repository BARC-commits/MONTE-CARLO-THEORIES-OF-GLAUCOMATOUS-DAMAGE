# Integrated Glaucoma Theory Model: A Monte Carlo Sensitivity Analysis

This repository contains a high-fidelity **Monte Carlo simulation of 1,000,000 virtual eyes**. The model evaluates how shifting assumptions and weightings across three primary pathophysiological frameworks—**Mechanical, Vascular, and Glymphatic theories**—impact predicted Intraocular Pressure (IOP) thresholds and subsequent glaucoma classifications.

---

## 📌 Core Finding: Sensitivity to Assumptions

The core takeaway of this simulation is methodological: **the weightings of these disease mechanisms are arbitrary, and results vary substantially across different configurations.** * **Fragility of Single Models:** Mean IOP thresholds vary by >1 mmHg, and Glaucoma/Normal Tension Glaucoma (NTG) prevalence shifts by nearly 5 percentage points depending on how theories are weighted.
* **Clinical Implications:** Any conclusion or diagnostic threshold based on a single static weight configuration is fragile. This highlights the absolute necessity of validating multi-theory mathematical models against real-world clinical data.

---

## 🛠️ Features & Model Architecture

The simulation constructs a diverse virtual population ($n = 1,000,000$) utilizing realistic probability distributions for:
* **Demographics & Anatomy:** Age, Central Corneal Thickness (CCT), Corneal Hysteresis, Scleral Stiffness, and Lamina Cribrosa (LC) pore diameter.
* **Hemodynamics & Pressures:** Baseline IOP, Mean Arterial Pressure (MAP), and Cerebrospinal Fluid Pressure (CSFP).
* **Vulnerabilities:** Integrates systemic risk factors including sleep apnea, diabetes, hypertension, family history, and nocturnal hypotension.

It tests **5 distinct weight configurations** to equitably analyze model sensitivity without privileging any single theory.

---

## 📦 Dependencies

The script is written in Python 3 and requires the following data science and visualization libraries:

```bash
pip install numpy pandas matplotlib
```
---

## 🚀 Usage

Simply clone the repository and run the Python script. The simulation will execute the 1-million-eye array operations using vectorized NumPy functions and save five publication-quality figures directly to your directory.

```bash
git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
cd YOUR_REPOSITORY_NAME
python glaucoma_simulation.py

```

### Generated Outputs:

1. `figure1_theory_thresholds.png` – Distribution of individual and integrated theory thresholds.
2. `figure2_vulnerability_scores.png` – Density mapping of population vulnerability by mechanism.
3. `figure3_sensitivity_to_weights.png` – Prevalence changes across weight configurations.
4. `figure4_vulnerability_vs_threshold.png` – Scatter analysis mapping combined vulnerability against age and IOP.
5. `figure5_threshold_variation.png` – Box plots highlighting threshold variance.

---

## 📋 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE).

```

```
