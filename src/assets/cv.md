# Kaustav Deka

**Bloomington, Indiana** · mailerdeka@gmail.com · +1-812-320-6318  
[LinkedIn](https://linkedin.com/in/dekak) · [GitHub](https://github.com/deka27)

---

## Summary

Data-focused engineer building reproducible Python pipelines and performance-optimized algorithms for diffusion MRI analysis. Experience shipping scientific software in open source (DIPY) and accelerating tractography through parallelization and Cython. Research spans brain microstructure estimation, cross-modality MRI synthesis, and uncertainty-adaptive tractography. Seeking applied machine learning / computer vision roles in medical imaging with strong experimentation, evaluation, and optimization practices.

---

## Education

**Master of Science in Intelligent Systems Engineering**  
Indiana University, Bloomington — GPA: 3.85 / 4.00 · Jan 2025 – Present  
Relevant Coursework: Machine Learning, Deep Learning, Computer Vision, Optimization, Information Visualization

**Bachelor of Engineering in Industrial Engineering & Management**  
Bangalore Institute of Technology, Bangalore, India · Aug 2015 – Jul 2019

---

## Skills

**Core:** Python, SQL, PyTorch, scikit-learn, NumPy, Pandas, SciPy  
**Modeling & Evaluation:** Model development, experimentation, hyperparameter optimization, statistical testing (Wilcoxon, ablation studies), Matplotlib, Seaborn  
**Deep Learning:** U-Net, Attention U-Net, Pix2Pix (cGAN), conditional VAE, mixed-precision training (AMP), loss function design (L1, SSIM, LSGAN, KL divergence)  
**Medical Imaging / Scientific Computing:** Diffusion MRI, tractography, cross-modality MRI synthesis (T1↔T2), DIPY neuroimaging library, FURY visualization library, NIfTI processing, parallel computing, OpenMP, Cython  
**Evaluation & Metrics:** PSNR, SSIM, MAE, LPIPS, FID, DICE, CNR, frequency analysis, robustness analysis  
**Tools:** Bash, Git, Docker, CI/CD, PyQt/PySide, Azure DevOps, Power BI, Blender, Gephi

---

## Experience

### Research Assistant
**Garyfallidis Research Group, Indiana University** · Bloomington, IN · Jan 2025 – Present

- Accelerated EuDX tractography by 12×, reducing runtime from hours to minutes via OpenMP parallelization and Cython optimization for large diffusion MRI datasets
- Built an end-to-end diffusion MRI pipeline using 15+ DIPY methods and a Bash CLI, automating 20+ steps previously executed manually
- Delivered a PyQt GUI that reduced DIPY setup complexity by 60%, enabling non-technical users to run advanced tractography workflows without command-line expertise
- Developed the GLIDE uncertainty-adaptive tractography algorithm within DIPY's Cython propagator architecture; evaluated on HCP data with RecoBundles across 80 bundles
- Contributed to the FORCE microstructure estimation pipeline (under review at *Nature Methods*), designing stability experiments including library resampling, neighborhood concentration analysis, and input perturbation
- Created publication-quality scientific figures: Nature-style SVG pipeline diagrams, multi-panel matplotlib comparison figures (FORCE vs. AMICO, DTI vs. FORCE for FA/MD/RD), and Blender-rendered white matter microstructure visualizations

### Google Summer of Code Contributor
**DIPY Neuroimaging Library (Diffusion Imaging in Python)** · Remote · Jan 2024 – Sep 2024

- Shipped 50+ open-source contributions to a Python library used by 10,000+ users, including performance improvements cutting memory use by 30% for typical workflows
- Implemented lazy loading to decrease import time by 45% and reduce initial memory footprint from 250 MB to 140 MB
- Improved documentation usability by refactoring a website serving 5,000+ monthly visitors, reducing developer onboarding time by 25%

### Senior Program Engineer
**RGBSI** · Bengaluru, India · Jan 2022 – Feb 2023

- Improved product adoption by 20% by building Power BI analytics dashboards to guide data-driven feature prioritization for a SaaS platform
- Delivered 4 enterprise software implementations for 200+ end users on schedule, achieving 95%+ stakeholder satisfaction

### Implementation Engineer
**RGBSI** · Bengaluru, India · Mar 2020 – Jan 2022

- Built 25+ Power BI and Business Objects dashboards analyzing historical trends, driving 3 major system enhancements and 15% efficiency gains
- Reduced production support tickets by 35% through proactive analysis and system gap identification, improving overall platform stability

---

## Publications

**FORCE: FORward modeling for Complex microstructure Estimation**  
Co-author · Under review at *Nature Methods* · [Preprint on ResearchSquare]  
Novel forward modeling approach for estimating brain tissue microstructure from diffusion MRI data. Contributed stability experiments, figure design, and pipeline validation.

**Cross-Modality Brain MRI Synthesis: A Comparative Study of Regression, Adversarial, and Variational Approaches for T1–T2 Translation**  
Atharva Shah\*, **Kaustav Deka**\* (\*co-first authors) · Indiana University Bloomington  
Comparative study of five deep learning architectures for bidirectional T1↔T2 brain MRI synthesis with multi-metric evaluation and robustness analysis.

---

## Projects

### Cross-Modality Brain MRI Synthesis (T1↔T2)
**Technologies:** PyTorch, NumPy, SciPy, Matplotlib  

- Benchmarked five architectures (U-Net, Attention U-Net, Pix2Pix, cVAE) for bidirectional T1↔T2 synthesis on 577 subjects from the IXI dataset
- Achieved 32.35 dB PSNR (Att-UNet) and FID of 13.6 (Pix2Pix), with a 13-experiment robustness suite probing lesion sensitivity, noise tolerance, and clinical safety

### SLAM with Extended Kalman Filter
**Technologies:** NumPy, SciPy, Pandas, Matplotlib, FURY · [GitHub](https://github.com/deka27/slam)

- Implemented SLAM with EKF achieving real-time state estimation at 30 Hz update rate
- Developed sensor fusion models handling uncertainty propagation with <5 cm localization error on benchmark datasets

### DIPY Workshop 2026 — Organizing Team
- Built the workshop's Learning Management System (LMS) for participant onboarding, content delivery, and progress tracking
- Contributed to event management including registrant processing, teleprompter scripts, and presentation materials

### HRA CloudFront Logs Analytics Dashboard
**Technologies:** Next.js, DuckDB, ECharts  

- Built an analytics dashboard analyzing 15M+ AWS CloudFront log records for the Human Reference Atlas project
- Designed interactive visualizations for traffic patterns, geographic distribution, and usage trends

### Career Builder Assistant (Personal Project)
**Technologies:** React, Vite, FastAPI, local-first flat-file storage  

- Designing a personal learning management app for tracking career development, skill progression, and learning goals

---

## Certifications & Activities

- **Google Summer of Code 2024** — DIPY (Diffusion Imaging in Python)
- **National Gold Medalist** — Karate (Black Belt)
- **DIPY Workshop 2026** — Organizer and Host
- **Badminton** — Active recreational player

---

## Technical Highlights

- **Performance Engineering:** 12× tractography speedup via OpenMP/Cython; 45% import time reduction via lazy loading; 30% memory reduction in DIPY workflows
- **Scientific Computing:** End-to-end diffusion MRI pipelines, multi-tensor signal modeling, ODF estimation, fiber peak extraction, microstructure estimation
- **Deep Learning for Medical Imaging:** Image-to-image translation (U-Net, Pix2Pix, cVAE), perceptual loss functions (LPIPS, FID), mixed-precision training, robustness evaluation
- **Evaluation Rigor:** Multi-metric evaluation frameworks, Wilcoxon signed-rank tests, ablation studies, frequency-domain analysis, uncertainty quantification
- **Visualization:** Publication-quality figures (Nature-style), Blender 3D rendering, Power BI dashboards, interactive web dashboards (ECharts, D3)