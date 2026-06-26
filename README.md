# 🧠 Robust Hippocampal-Striatal Recruitment During Auditory Processing

**Neuroscience Research Project – Sharif University of Technology**  
- 👨‍💻 **Author:** Moein Yousefinia
- 👨‍🏫 **Supervisor:** Prof. Hamid K. Aghajan

---

## 📁 Repository Structure

```text
📦 root/
├── 📁 Project_Data/                # Raw LFP and event matrices
│   ├── 📄 EventMatrix.mat          # Event markers (Standard vs. Target)
│   └── 📄 LFPData.mat              # Continuous Local Field Potential data
├── 📄 code.ipynb                   # Main analysis notebook (PAC & Granger Causality)
├── 📄 features_pac.npy             # Extracted Phase-Amplitude Coupling feature matrix
├── 📄 Final_Results.png            # GC visualizations and statistical outputs
├── 📄 Result_Figure_PAC.png        # Temporal dynamics of PAC (HC -> dS)
├── 📄 Neuro_Project.pdf            # Full research paper and methodology
└── 📄 README.md                    # Project overview & instructions
🧩 Project OverviewThe brain's ability to detect and adapt to novel stimuli is fundamental for survival. This research investigates the dynamic network interactions underlying novelty processing, focusing specifically on the directional communication between the Hippocampus (HC) and Dorsal Striatum (dS).Using Local Field Potential (LFP) recordings from an auditory oddball task, this study questions whether the neural processing of novelty is mediated by a transient reorganization of information flow in these circuits.🎯 Objectives & MethodologyLFP Analysis: Analyzed neural activity from the Hippocampus, Dorsal Striatum, and mPFC during a passive auditory oddball task.Phase-Amplitude Coupling (PAC): Computed Theta (4-8 Hz) to Gamma (30-80 Hz) coupling using Mean Vector Length (MVL) over 200 ms sliding windows to quantify cross-regional communication.Directional Causality: Applied Granger Causality (GC) to test whether past values of the Hippocampus predict future values of the Dorsal Striatum ($HC\rightarrow dS$).Statistical Testing: Compared information flow between Standard and Target (novel) conditions using Welch's t-test across temporal windows.🔑 Key FindingsRobust Temporal Modulation: Identified a massive surge in PAC strength starting 130 ms post-stimulus and peaking at 330-730 ms, aligning with the P300 cognitive processing timeframe.Non-Selective Response: Contrary to the novelty-filter hypothesis, the HC-dS network was recruited equally for both Standard and Target stimuli, with no statistically significant difference $(p>0.05)$.Theoretical Implication: The findings suggest this hippocampal-striatal loop is recruited for general temporal integration rather than acting as a purely novelty-gated filter in passive settings.🛠️ Technologies UsedPython (Jupyter Notebook)SciPy & Statsmodels (For advanced statistical testing and GC feature extraction)NumPy (For .npy feature matrix manipulation and time-series processing)Matplotlib (For temporal trajectory visualizations)🧪 How to RunClone the repository and open the main notebook to view the pipeline:Bash# Clone the repository
git clone [https://github.com/moein-yoo/LFP-Novelty-Network-Dynamics.git](https://github.com/moein-yoo/LFP-Novelty-Network-Dynamics.git)
cd LFP-Novelty-Network-Dynamics

# Launch the main analysis notebook
jupyter notebook code.ipynb
Note: Ensure you have Project_Data/LFPData.mat and Project_Data/EventMatrix.mat in the correct directory before executing the cells.📜 Reports & Full PaperFor full theoretical explanations, mathematical formulations, and detailed discussion, please refer to the primary document:Neuro_Project.pdf – Robust Hippocampal-Striatal Recruitment During Auditory ProcessingAuthor Contact:Moein Yousefinia – moein.yoo84@sharif.edu | LinkedInThis repository shifts the focus from localized ERP activation to dynamic functional connectivity, validating the use of LFP features to track real-time network reorganization during sensory processing.
