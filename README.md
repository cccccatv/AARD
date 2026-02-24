# AARD
# [CVPR 2026] AARD: Geometry-Aligned and Anomaly-Aware Reconstruction for 3D Anomaly Detection

Official implementation of the paper "**AARD: Geometry-Aligned and Anomaly-Aware Reconstruction for 3D Anomaly Detection**".

---

## 📢 News
* **[2026-02-21]** Paper accepted by CVPR 2026! 🚀
* **[Coming Soon]** We are cleaning up the code and checkpoints, and will release them shortly.

## 💡 Abstract
Point cloud anomaly detection is crucial in automated manufacturing, with reconstruction-based diffusion methods emerging as a mainstream solution. However, these approaches still face two major challenges: (1) geometry violation, where random noise perturbations deviate from local surface normals, causing structural distortion; and (2) undistinguished reference regions, where uniformly applied coarse anomaly embeddings during denoising blur normal details and impede accurate anomaly recovery. To address these issues, we propose AARD, a geometry-aligned and anomaly-aware diffusion reconstruction framework. We argue that high-fidelity anomaly detection requires a principled reformulation of the diffusion process: noise should align with geometry to preserve structures, and reconstruction can be better guided by anomaly-aware references to discriminatively recover normal details while correcting defects. AARD progressively aligns noise directions with vertex normals while maintaining vertex-graph consistency, and employs an adaptive transformer that assigns normal references to anomalous regions and input references to normal areas. Experiments on Anomaly-ShapeNet and Real3D-AD show that AARD consistently outperforms state-of-the-art approaches, achieving superior geometric fidelity and robust anomaly localization.




## 🛠️ TODO List
- [ ] Release inference code and pre-trained weights.
- [ ] Release training scripts for MVTec 3D-AD and Real3D-AD.
- [ ] Detailed documentation and environment setup (Docker/Conda).

## 📝 Citation
If you find our work useful, please consider citing:
```bibtex
@inproceedings{wang2026aard,
  title={AARD: Geometry-Aligned and Anomaly-Aware Reconstruction for 3D Anomaly Detection},
  author={Linchun Wu，Qin Zou， Yuanhao Yue and Zhongyuan Wang}},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year={2026}
}
