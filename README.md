# DepthFusionNet

### A Transformer-Based Hybrid Architecture for Monocular Depth Estimation Using Local-Global Feature Fusion

**Author:** Pankaj Kumar Gautam  
**Email:** pankajgautam257@gmail.com  
**Affiliation:** Department of Computer Science and Engineering, United University, Prayagraj, India  

---

## 🧠 Overview
**DepthFusionNet** is a transformer-based hybrid model for **monocular depth estimation (MDE)**.  
It combines global context learning through transformer encoders with local detail refinement using a convolutional decoder.  
The architecture employs a **Selective Feature Fusion (SFF)** module and an **Attention-Supervised Upsampling (ASU)** block to improve depth boundary sharpness and structural consistency.

This repository accompanies the research paper:  
> *A Transformer-Based Hybrid Architecture for Monocular Depth Estimation Using Local-Global Feature Fusion* — Pankaj K. Gautam, Sanjeev Kumar.

---

## 🚀 Key Features
- **Hybrid Transformer–CNN Architecture**: Efficient encoder-decoder design with rich spatial semantics.
- **Selective Feature Fusion (SFF)**: Fuses local and global features adaptively for multi-scale representation.
- **Attention-Supervised Upsampling (ASU)**: Enhances depth precision at edges and boundaries.
- **Depth-Aware Augmentation**: Boosts model robustness under varying indoor and outdoor conditions.
- **Cross-Domain Generalization**: Evaluated on NYU Depth V2 and VS13 datasets.

---

## 📂 Datasets
| Dataset | Scene Type | Resolution | Usage | Notes |
|----------|-------------|-------------|--------|--------|
| **NYU Depth V2** | Indoor | 640×480 | Quantitative | Standard benchmark (Eigen split, center-cropped to 320×240) |
| **VS13** | Outdoor (Traffic) | Varies | Qualitative | Cross-domain generalization study |
| **KITTI, DIODE, Make3D** | Mixed | – | Optional | For extended validation |

---

## ⚙️ Installation
```bash
# clone the repository
git clone https://github.com/<your-username>/DepthFusionNet.git
cd DepthFusionNet

# create and activate virtual environment
python -m venv venv
source venv/bin/activate   # on Windows: venv\Scripts\activate

# install dependencies
pip install -r requirements.txt
