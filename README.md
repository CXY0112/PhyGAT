# PhyGAT
This repository contains the implementation code of the PhyGAT framework proposed in our paper "Optimizing Physics-Informed Neural Networks with Graph Attention: A Lightweight and Efficient Framework for Solving PDEs". PhyGAT combines Graph Attention Networks (GATs) with Physics-Informed Neural Networks (PINNs) to solve one-dimensional partial differential equation (PDEs) problems in an efficient and lightweight manner.

# Main Contributions
The main contributions of our research include: 

We introduce a novel framework PhyGAT that integrates GATs to dynamically model physical interactions via attention mechanisms, significantly enhancing the model's expressive power;

Compared to vanilla PINNs and Robust Weight Initialization PINNs, our approach a 20× speedup in inference and reduces parameter count by 49×, enabling efficient deployment on resource-constrained devices;

Extensive evaluations across three diverse classes of 1D PDEs, including nonlinear and time-dependent systems, our method achieves an order-of-magnitude improvement in predictive accuracy.

# Repository Structure
```
PhyGAT
├── data/                     # Ground truth data
│   ├── Allen_Cahn.npz           
│   ├── convection_equation.npz  
│   └── diffusion.npz         
├── result/                   # Training result
│   ├── Allen_Cahn_PhyGAT/
│   │   ├── losses.txt         
│   │   └── pred_val.npy       
│   ├── Convection_PhyGAT/
│   │   ├── losses.txt         
│   │   └── pred_val.npy       
│   └── Diffusion_PhyGAT/
│       ├── losses.txt         
│       └── pred_val.npy       
├── requirements.txt            
├── PhyGAT_ALLEN-Cahn.ipynb     # Allen-Cahn equation experiment
├── PhyGAT_Convection.ipynb     # convection equation experiment
└── PhyGAT_diffusion.ipynb      # diffusion equation experiment

```
