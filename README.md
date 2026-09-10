<div align="center">

# Benhuang Liu

**Computer Vision · Reliable Visual Learning · Embodied Perception**

M.S. student, [Waseda University — Graduate School of Information, Production and Systems](https://www.waseda.jp/fsci/gips/en/)  
September 2026 intake

B.Sc. in Computer Science, [Macau University of Science and Technology](https://www.must.edu.mo/)

</div>

## Research

I am interested in how vision systems behave when the evidence is imperfect: when an image is 4K and degraded, an RGB-D match is ambiguous, or a robot should abstain instead of acting on a weak prediction.

My undergraduate work centered on ultra-high-definition image restoration. More recently, I have been exploring confidence-aware RGB-D correspondence and vision-guided robotic manipulation. My current interests include **image restoration and generative vision**, **RGB-D and 3D perception**, and **vision-language models for embodied systems**.

## Selected projects

### [GatedResidual — confidence-aware output blending for UHD restoration](https://github.com/steinsgo/Resblock-For-UHDprocesser)

`Final-year project` · `PyTorch` · `4K image restoration`

A lightweight spatial gate for degradation-conditioned all-in-one restoration. It blends the network output with the original input when the selected restoration route is unreliable. The module adds **11,107 parameters (0.6% overhead)**. In deliberate misclassification stress tests, it recovered **10.13 dB on average** over the ungated wrong-route output; the nominal-quality trade-off is reported alongside the robustness result.

### [Confidence-aware RGB-D correspondence for unseen-object pose](https://github.com/steinsgo/rgbd-confidence-pose/tree/agent/readme-quality-gate)

`Independent study — ongoing` · `RealSense D435i` · `DINOv2 / SIFT` · `SE(3)`

An end-to-end pipeline for RGB-D session validation, 2D-to-3D correspondence, confidence-aware RANSAC, and Kabsch refinement. A known-pose synthetic test reached **0.084° rotation error** and **1.6 mm translation error**. Real D435i recordings have been used for integrity and matching checks; independent real-pose ground truth remains the main open requirement.

### [ConfMate — confidence-gated visual matching for robotic insertion](https://github.com/steinsgo/vlm-robot-color-sorting/tree/confmate-baseline)

`Simulation study — ongoing` · `PyBullet` · `CLIP` · `Franka Panda`

A reproducible peg-hole matching and manipulation prototype with multi-view Chamfer/CLIP baselines, confidence-based abstention, partial-observation evaluation, and a four-object Panda mission. The project keeps oracle control tests separate from actual visual matching results.

## Other builds

- [**DepthForce**](https://github.com/steinsgo/depthforce) — a CUDA particle-interaction prototype driven by depth motion, with a D435i input path and a 150k-particle synthetic mode running at 119–122 FPS on an RTX 3060 Laptop GPU.
- [**Ancient Character OCR**](https://github.com/steinsgo/DanC) — a containerized full-page rubbing-image pipeline using YOLO11m for character detection and ResNet50 for glyph recognition.

## Tools I use

Python · PyTorch · OpenCV · DINOv2 · Transformers · ROS 2 · PyBullet · NVIDIA Warp/CUDA · Intel RealSense

---

<sub>Away from the GPU: electric guitar, fusion and modern jazz, games, and street photography.</sub>
