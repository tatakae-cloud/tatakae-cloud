# Sai Ganesh Upadrasta
Integrated M.Tech — International Institute of Information Technology Bangalore (IIITB)

---

# Experience

## Research Intern — E-Health Research Center (EHRC), IIIT Bangalore & NIMHANS
Jun 2026 – Present
Patient Trajectory Modeling using Transformers
Repository: https://github.com/IIITBangalore/brainCohort-diseaseTrajectory-b4b

- Reimplemented Delphi-2M, an autoregressive transformer for patient disease trajectory modeling, with dual heads for next-ICD-10-code prediction and time-to-event regression; trained on dual-GPU with DataParallel mixed-precision (2.24M parameters, 12 layers, 12 heads).
- Evaluated model generalization across 138 ICD-10 codes on a real-world clinical cohort, achieving 0.656 mean AUC and 0.786 AUC for mortality prediction, against the original paper's 0.76 AUC trained on the Danish Registry (1.93M individuals, 56x larger).
- Extended the model with generative trajectory sampling using learned hazard rates for future visit simulation, validated with 0.701 Pearson correlation for ages 70–75; analyzed comorbidity feature impacts via a SHAP-based matrix.

---

## Research Intern — Lab for Spatial Informatics, IIIT Hyderabad
Aug 2025 – Dec 2025
Cloud-Free Satellite Image Reconstruction
Repository: https://github.com/svnsaisathvik/Cloud-Removal

- Built a cloud removal pipeline for Sentinel-2 multispectral imagery using physics-based per-pixel validity masks and exponential decay temporal weighting to reconstruct cloud-occluded regions, achieving 0.9137 SSIM (32.67 dB PSNR).
- Trained a residual U-Net on 26K spatial patches over 80 epochs with a combined L1 and MSE loss to refine temporally aggregated reconstructions, maintaining stable convergence on full-resolution 5000×5000 pixel scenes.
- Engineered a tiled inference pipeline with temporal sorting and weighted aggregation to process large-scale satellite scenes up to 25M pixels end-to-end without memory overflow.

---

## Research Intern — Yashoda Hospitals
Aug 2025 – Dec 2025
Multi-Label Chest X-Ray Classification
Repository: https://github.com/tatakae-cloud/Aug-CNN-

- Built 3-branch attention-guided CNN architecture for chest X-ray diagnosis.
- Achieved 0.760 mean AUC across 14 pathologies on 12,120 chest X-rays.
- Designed 3-stage training pipeline improving calibration and stability.
- Implemented attention heatmap extraction for radiologist-interpretable predictions.

---

# Projects

## Fine-Tuning IBM TerraMind ViT Foundation Model for Cloud Removal
Repository: https://github.com/svnsaisathvik/Cloud-Removal

- Fine-tuned IBM TerraMind Vision Transformer for Sentinel-2 cloud removal.
- Built 12-band multispectral data pipeline using Rasterio.
- Implemented pixel-wise regression training for cloud reconstruction.
- Added TensorBoard logging and reproducible training pipelines.

---

## SFDLCS — Deep Learning Compressive Sensing for UWB Signal Reconstruction
Repository: https://github.com/tatakae-cloud/sfdlcs-uwb-reconstruction

- Replicated SFDLCS end-to-end with manual LSTM gates (Eq. 3–9) and FCNN decision network on 2,000 synthetic UWB signals; achieved 59% lower NMSE vs. OMP, 35% vs. BCS, and 24% vs. GPSR on 400 test signals.
- Proposed Transformer-based search network (2-layer encoder, 4-head self-attention, d=128) replacing paper's LSTM, reducing NMSE by 8% and raising correct index recovery rate to 93% (14/15 per signal).
- Benchmarked 5 algorithms (SFDLCS, SFDLCS-Transformer, OMP, BCS, GPSR) across 10 SNR levels (-20 to +40 dB); SFDLCS maintained lowest NMSE across entire noise range, validating robustness claims.

---

## StackConnect — Full-Stack Developer Networking Platform
Apr 2026 – May 2026
Repository: https://github.com/KhSudhir2345/Buildathon-2.0---Actual
Live: https://buildathon-2-0-actual.vercel.app/

- Developed a full-stack developer networking platform using React, Node.js, Express, and MongoDB, featuring JWT-based authentication, profile management, and secure REST APIs.
- Designed a skill-based matchmaking engine with fuzzy skill normalization, category expansion, and ranking algorithms to improve discovery of relevant developer connections.
- Implemented real-time messaging and networking workflows using Socket.IO, enabling instant chat, swipe-style interactions, and live user updates on a responsive TailwindCSS interface.

---

## Academia Portal — Concurrent Client-Server Course Registration System
Mar 2025 – May 2025
Repository: https://github.com/tatakae-cloud/academia-portal-course-registration-system

- Built a multi-threaded client-server academic course registration system in C using TCP sockets, supporting role-based access for Admin, Faculty, and Student users.
- Implemented concurrent client handling with POSIX threads and mutex-based synchronization, ensuring safe access to shared student, faculty, and course records under simultaneous requests.
- Designed persistent storage using low-level Unix system calls and developed enrollment, seat-allocation, authentication, and course-management workflows with signal-based graceful shutdown support.

---

## NASA Log Analytics — Multi-Engine Big Data Pipeline
Jan 2026 – May 2026
Repository: https://github.com/ashokCh-dev/No_Sql_final_project

- Architected a 4-pipeline analytics framework (Hadoop MapReduce, MongoDB, Pig, Hive) over 1.89M NASA HTTP log records (196 MB), with a unified PostgreSQL result schema and Python CLI supporting 12 pipeline×query combinations.
- Implemented 3 analytical queries (daily traffic, top-20 resources, hourly error analysis) across all pipelines with byte-identical output; stream-processed in 50K-record batches and handled 2,048 malformed records via a shared regex parser.
- Benchmarked all 4 engines on the full dataset: MongoDB (26s) achieved 7× speedup over MapReduce (183s); traced Pig's 1,076s runtime to per-query JVM cold-starts and YARN container serialization overhead.

---

# Technical Skills

Languages
Python • C • C++ • Java • JavaScript

Frameworks
PyTorch • TensorFlow • PyTorch Lightning • Scikit-learn • React • Express.js • Node.js

Databases
MongoDB • MySQL • PostgreSQL • SQL • NoSQL

Tools
Git • Linux • Socket Programming • POSIX Threads • TensorBoard • Google Earth Engine • Rasterio • NumPy • Pandas • Matplotlib • Hadoop • MapReduce • Pig • Hive • TerraTorch
