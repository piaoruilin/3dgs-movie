# 3D Gaussian Splatting Reconstruction

This repository contains the full pipeline and implementation for creating a short animated mini-movie using dynamic 3D Gaussian Splatting (3DGS). The project includes data capture, 3D reconstruction, scene and object modeling, dynamic sequence design, and rendering. All reconstruction and training were performed using Google Colab with Python 3.11+ and the `gsplat`/Nerfstudio toolset. 
Korea University Course DATA302 - Computer Vision and Its Applications (기초컴퓨터비전과응용)
---

## 1. Overview

The goal of this project is to reconstruct a real-world environment and multiple physical objects from video and render them entirely with 3D Gaussian Splatting.

This pipeline includes:

- Video capture and preprocessing  
- Frame extraction  
- COLMAP-based structure-from-motion reconstruction  
- Training Gaussian Splatting models for one scene and multiple objects  
- Inserting and animating reconstructed objects inside a reconstructed scene  
- Designing camera motion and object transformations  
- Rendering a final animated sequence

---

## 2. Dependencies

```bash
!pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
!pip install nerfstudio gsplat
```
## 3. References

Kerbl et al., "3D Gaussian Splatting for Real-Time Radiance Field Rendering"
Nerfstudio Documentation: https://docs.nerf.studio
gsplat Repository: https://github.com/nerfstudio-project/gsplat
