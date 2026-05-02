# NeuroGuard AI: Explainable 3D Vision Transformer Framework
![Python](https://img.shields.io/badge/Python-3.10-blue) ![PyTorch](https://img.shields.io/badge/PyTorch-2.0-red) ![BraTS2023](https://img.shields.io/badge/Dataset-BraTS2023-green) ![License](https://img.shields.io/badge/License-MIT-yellow)

## Automated 3D Brain Tumor Segmentation & Clinical Decision Support

NeuroGuard AI is an advanced medical imaging solution designed to detect and segment brain tumors from multi-modal MRI scans. By leveraging hierarchical **Vision Transformers**, it provides clinicians with high-precision segmentation masks, 3D volumetric reconstructions, and explainable AI insights.

---

## 🎬 Project Showcase
### **System Dashboard & 3D Reconstruction**
<img width="100%" alt="NeuroGuardAI_Dashboard_main" src="https://github.com/user-attachments/assets/f110e909-cd4c-469e-8413-e4b451a3d96a" />

> **Watch the Full Video Demo:** [Clinical Workflow & 3D Visualization](https://drive.google.com/file/d/15-E95hjJL6tW3fxZo9seBLfxuh2xjIlM/view?usp=drive_link)

---

## 🏗️ Technical Architecture & Pipeline
NeuroGuard AI utilizes a hybrid Transformer-CNN architecture to capture both local fine-grained details and global spatial dependencies.

<img width="100%" alt="NeuroGuardAI_demo_architecture_main" src="https://github.com/user-attachments/assets/59aa9bd2-58b8-472a-87f7-233f640cfb59" />

### Key Architectural Components:
*   **Hierarchical Swin Encoder:** Uses shifted windowing to compute self-attention across 3D volumes while maintaining linear computational complexity.
*   **Feature Fusion:** Employs skip connections between the Transformer encoder and CNN decoder to preserve sharp spatial boundaries of irregular tumors.
*   **Reliability Engineering:** Implements Monte Carlo Dropout (10 stochastic passes) to quantify epistemic uncertainty for clinical decision support.
*   **3D Reconstruction:** Converts voxel probability maps into high-fidelity meshes using the Marching Cubes algorithm.

---

## 🩺 Clinical Impact & Utility
Designed to bridge the gap between "Black-Box" AI and surgical planning:
*   **Volumetric Precision:** Provides exact measurements of Tumor Core and Edema in $cm^3$ for longitudinal tracking.
*   **Risk Assessment:** Automated triage flags based on pathological urgency (Immediate/Consultation).
*   **Surgeon-Ready Reports:** Generates standardized PDF reports including slice-by-slice analysis and 3D tumor mapping.
*   **Sample Output:** [View Sample Clinical Report (PDF)](https://github.com/user-attachments/files/27304251/NeuroGuard_Sample_Report_main.pdf)

---

### 📊 System Performance & Capabilities
| Feature / Metric | Status / Value |
| :--- | :--- |
| **Model Architecture** | Swin-UNETR (63M Parameters) |
| **Training Dataset** | BraTS 2023 |
| **Inference Latency** | < 10 Seconds (RTX 4060) |
| **Global Mean Dice** | **0.7012** (Validation, BraTS 2023) |
| **3D Reconstruction** | Dynamic Mesh Generation via Marching Cubes |
| **Clinical Output** | Automated PDF Volumetric Reporting |

---

## 🛠️ Tech Stack
*   **Language:** Python
*   **Deep Learning:** PyTorch, MONAI (Medical Open Network for AI)
*   **Data Processing:** NumPy, Nibabel, Scikit-image
*   **Interface:** PyQt6 Desktop Application

---

## 📂 Repository Structure & Privacy
> **Note:** This repository is a public showcase for architectural overview and results. To protect intellectual property and ongoing research publication, the full source code is maintained in a private repository.

---

## 🤝 Contact & Collaboration
*   **Developer:** Jugal S Brahmkshatriya
*   **LinkedIn:** [linkedin.com/in/jugal-brahmkshatriya](https://linkedin.com/in/jugal-brahmkshatriya)
*   **GitHub Profile:** [github.com/Jugalbrahmkshatriya](https://github.com/Jugalbrahmkshatriya)
