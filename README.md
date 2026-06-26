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
```
## 🧩 Project Overview

The brain's ability to detect and adapt to novel stimuli is fundamental for survival. This research investigates the dynamic network interactions underlying novelty processing, focusing specifically on the directional communication between the Hippocampus (HC) and Dorsal Striatum (dS).

Using Local Field Potential (LFP) recordings from an auditory oddball task, this study questions whether the neural processing of novelty is mediated by a transient reorganization of information flow in these circuits.

## 🎯 Objectives & Methodology

- **Experimental Setup:** Analyzed continuous Local Field Potential (LFP) signals extracted from the Hippocampus, Dorsal Striatum, and mPFC during a passive auditory oddball paradigm.
- **Functional Connectivity (PAC):** Quantified cross-regional communication by calculating Phase-Amplitude Coupling (PAC). Specifically, we evaluated how Hippocampal Theta phase (4-8 Hz) modulates Gamma amplitude (30-80 Hz) using the Mean Vector Length (MVL) metric across 200 ms non-overlapping sliding windows[cite: 1].
- **Directionality Tracking:** Deployed **Granger Causality (GC)** to explicitly test the directional flow of information, evaluating whether past hippocampal activity effectively predicts future striatal states ($HC\rightarrow dS$)[cite: 1].
- **Statistical Evaluation:** Conducted rigorous hypothesis testing using Welch’s independent t-test to compare temporal network dynamics between standard and target (novel) auditory sequences[cite: 1].

---

## 🔑 Key Findings

- **Late-Latency Network Surge:** Discovered a highly robust, time-locked spike in Hippocampal-Striatal connectivity peaking between 330 and 730 ms post-stimulus[cite: 1]. This activation closely aligns with the temporal window of the P300 cognitive component[cite: 1].
- **General Integration Over Selective Filtering:** Statistical analyses revealed identical coupling trajectories for both novel and standard stimuli, with no significant differences in peak PAC strength $(p=0.49)$ or Granger Causality scores $(p=0.435)$[cite: 1].
- **Redefining Circuit Role:** The findings challenge the assumption that the HC-dS pathway acts purely as a novelty-gated filter in passive settings[cite: 1]. Instead, the data suggests this circuit continuously facilitates baseline orienting and temporal integration of all incoming sensory inputs[cite: 1].

---

## 🛠️ Technologies Used

- **Environment:** Python (Jupyter Notebook)
- **Signal Processing & Statistics:** `SciPy` and `Statsmodels` for feature extraction (Hilbert transform), Granger Causality computation, and statistical hypothesis testing.
- **Data Handling:** `NumPy` for managing large, multi-dimensional LFP arrays and `.npy` feature matrices[cite: 1, 2].
- **Visualization:** `Matplotlib` for generating temporal trajectories, error bars, and comparative network plots[cite: 2].

---

## 🧪 How to Run

To replicate the analyses or explore the feature extraction pipeline:

```bash
# Clone the repository
git clone [https://github.com/moein-yoo/LFP-Novelty-Network-Dynamics.git](https://github.com/moein-yoo/LFP-Novelty-Network-Dynamics.git)
cd LFP-Novelty-Network-Dynamics

# Launch the main analysis notebook
jupyter notebook code.ipynb
```

## 📜 Research Paper & Documentation

For a comprehensive exploration of the theoretical framework, mathematical modeling of functional connectivity, and detailed neurophysiological interpretations, please consult the complete manuscript:
- 📄 [**Robust Hippocampal-Striatal Recruitment During Auditory Processing: A Non-Selective Response to Novelty**](Neuro_Project.pdf)[cite: 1, 2]

---

## 📬 Author & Contact

**Moein Yousefinia**  
*Electrical Engineering Department, Sharif University of Technology*[cite: 1]  
- 📧 **Email:** [moein.yoo84@sharif.edu](mailto:moein.yoo84@sharif.edu)[cite: 1]
- 🔗 **LinkedIn:** [Moein Yousefinia](https://linkedin.com/in/moein-yousefinia-335269284)
- 💻 **GitHub:** [moein-yoo](https://github.com/moein-yoo)

> *By shifting the analytical focus from localized activation (ERPs) to dynamic, time-resolved information flow, this repository provides a methodological framework for mapping real-time network reorganization in deep-brain structures during cognitive tasks.*
