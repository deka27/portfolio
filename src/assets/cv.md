# Kaustav Deka

**Bloomington, Indiana** · mailerdeka@gmail.com · +1-812-320-6318  
[LinkedIn](https://linkedin.com/in/dekak) · [GitHub](https://github.com/deka27) · [Portfolio](https://deka27.github.io/portfolio/)

---

## Summary

Engineer working across machine learning, web, and data. Built open-source scientific software (DIPY), production analytics dashboards processing 30M+ records (Next.js / DuckDB), a Python LMS for an international workshop (FastAPI / HTMX), and performance-critical Cython algorithms for diffusion MRI. Open to applied ML, web, and product engineering roles.

---

## Education

**Master of Science in Intelligent Systems Engineering**  
Indiana University, Bloomington — GPA: 3.85 / 4.00 · Jan 2025 – Present  
Relevant Coursework: Machine Learning, Deep Learning, Computer Vision, Optimization, Information Visualization

**Bachelor of Engineering in Industrial Engineering & Management**  
Bangalore Institute of Technology, Bangalore, India · Aug 2015 – Jul 2019

---

## Skills

**Core:** Python, PyTorch, scikit-learn, NumPy, SciPy  
**Deep Learning:** U-Net, Attention U-Net, Pix2Pix (cGAN), conditional VAE, mixed-precision training (AMP), loss function design (L1, SSIM, LSGAN, KL divergence)  
**Scientific Computing:** Diffusion MRI, tractography, DIPY, FURY, NIfTI processing, OpenMP, Cython, parallel computing  
**Data:** SQL, Pandas, DuckDB, Power BI, Business Objects, Matplotlib, Seaborn  
**Web:** React, Next.js, Vite, Astro, FastAPI, HTMX, ECharts, D3, Tailwind, TypeScript  
**Product:** Azure DevOps, feature prioritization, stakeholder management, SaaS analytics  
**Tools:** Git, Docker, CI/CD, Bash, PyQt/PySide, Blender, Gephi  
**Evaluation & Metrics:** PSNR, SSIM, MAE, LPIPS, FID, DICE, CNR, Wilcoxon signed-rank, ablation studies, frequency analysis

---

## Experience

### Research Assistant
**Garyfallidis Research Group, Indiana University** · Bloomington, IN · Jan 2025 – Present

- Accelerated EuDX tractography by 12×, reducing runtime from hours to minutes via OpenMP parallelization and Cython optimization for large diffusion MRI datasets
- Built an end-to-end diffusion MRI pipeline using 15+ DIPY methods and a Bash CLI, automating 20+ steps previously executed manually
- Delivered a PyQt GUI that reduced DIPY setup complexity by 60%, enabling non-technical users to run advanced tractography workflows without command-line expertise
- Developing the GLIDE uncertainty-adaptive tractography algorithm within DIPY's Cython propagator architecture; evaluated on HCP data with RecoBundles across 80 bundles
- Contributed to the FORCE microstructure estimation pipeline (under review at *Nature Methods*), designing stability experiments including library resampling, neighborhood concentration analysis, and input perturbation
- Built and ship the lab's web infrastructure: the Garyfallidis Research Group website (Sphinx) and the DIPY Workshop LMS (FastAPI / HTMX / PostgreSQL) for participant onboarding, content delivery, and progress tracking
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

### HRA & CNS Analytics Dashboard
**Technologies:** Next.js, TypeScript, Tailwind, ECharts, DuckDB, Python, Prophet, scikit-learn  
**Live:** [hra-viz.vercel.app](https://hra-viz.vercel.app) · **GitHub:** [deka27/hra-viz](https://github.com/deka27/hra-viz)

- Built a multi-dashboard analytics platform processing 31M+ AWS CloudFront records for two Indiana University projects — Human Reference Atlas (humanatlas.io) and Cyberinfrastructure for Network Science (cns.iu.edu)
- 13 dashboard pages with 70+ chart components spanning traffic, geography, content, errors, and ML insights
- ML pipeline: Prophet forecasting, churn prediction, error clustering (TF-IDF + KMeans), and bot detection (Isolation Forest) over 18 years of CNS traffic and 34 months of HRA traffic
- Data pipeline in DuckDB SQL on Parquet, with PubMed and GitHub API enrichment; 58 pytest data integrity tests; deployed via Vercel static export

### DIPY Workshop LMS
**Technologies:** FastAPI, HTMX, Jinja2, SQLAlchemy, PostgreSQL, Supabase, Redis  
**Live:** [workshop.dipy.org/lms](https://workshop.dipy.org/lms) · **GitHub:** [dipy/dipy_lms](https://github.com/dipy/dipy_lms)

- Built a Python LMS for the 2026 DIPY workshop with magic-link auth, role-based access (staff and watcher tiers), talks with resources, live chat with infinite-scroll history, threaded forum with markdown and image uploads, and Q&A
- CSV bulk user import with column mapping, year assignment, and per-row results; sliding-window rate limiting (Redis with in-memory fallback)
- Deployed to Indiana University infrastructure with systemd and supervisor; reverse-proxied behind nginx

### Cross-Modality Brain MRI Synthesis (T1↔T2)
**Technologies:** PyTorch, NumPy, SciPy, Matplotlib

- Benchmarked five architectures (U-Net, Attention U-Net, Pix2Pix, cVAE) for bidirectional T1↔T2 synthesis on 577 subjects from the IXI dataset
- Achieved 32.35 dB PSNR (Att-UNet) and FID of 13.6 (Pix2Pix), with a 13-experiment robustness suite probing lesion sensitivity, noise tolerance, and clinical safety

### Garyfallidis Research Group Website
**Technologies:** Sphinx, PyData Sphinx Theme, Python  
**Live:** [grg.luddy.indiana.edu](https://grg.luddy.indiana.edu) · **GitHub:** [deka27/grg-web](https://github.com/deka27/grg-web)

- Designed and built the public website for the Garyfallidis Research Group at Indiana University — research, team, publications, and blog
- Custom Sphinx theme and content management workflow

### SLAM with Extended Kalman Filter
**Technologies:** NumPy, SciPy, Pandas, Matplotlib, FURY · **GitHub:** [deka27/slam](https://github.com/deka27/slam)

- Implemented SLAM with EKF achieving real-time state estimation at 30 Hz update rate
- Developed sensor fusion models handling uncertainty propagation with <5 cm localization error on benchmark datasets

---

## Certifications & Activities

- **Google Summer of Code 2024** — DIPY (Diffusion Imaging in Python)
- **DIPY Workshop 2026** — Organizing Team (LMS, registrant processing, presentation materials)
- **Badminton** — Active recreational player

---

## Technical Highlights

- **Performance Engineering:** 12× tractography speedup via OpenMP/Cython; 45% import time reduction via lazy loading; 30% memory reduction in DIPY workflows
- **Scientific Computing:** End-to-end diffusion MRI pipelines, multi-tensor signal modeling, ODF estimation, fiber peak extraction, microstructure estimation
- **Deep Learning for Medical Imaging:** Image-to-image translation (U-Net, Pix2Pix, cVAE), perceptual loss functions (LPIPS, FID), mixed-precision training, robustness evaluation
- **Full-Stack Web:** Next.js + DuckDB analytics platforms (31M+ records), FastAPI + HTMX LMS, static-site generation (Astro, Sphinx), data visualization (ECharts, D3, Matplotlib)
- **Evaluation Rigor:** Multi-metric evaluation frameworks, Wilcoxon signed-rank tests, ablation studies, frequency-domain analysis, uncertainty quantification
