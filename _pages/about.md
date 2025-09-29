---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>
# Welcome! 
 I am a Master's student at the Beijing Institute of Technology, advised by Prof. <a href="https://scholar.google.cz/citations?user=0PJAjX4AAAAJ&hl">Shuxiang Guo</a>.  My research interests include LLM post-training,medical image analysis and surgical robotics. I have contributed to multiple projects in these areas, resulting in several publications in top-tier venues such as IEEE JSTARS, IEEE/ASME Transactions on Mechatronics, and MICCAI. 


# 📝 Publications 
<div class='paper-box'><div class='paper-box-image'><div><img src='images/5dof.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
<div class="badge">IEEE/ASME T-MECH (JCR Q1 IF 7.3)</div>
[5-DOF Micro-coil Positioning System Utilizing Single-axis Electromagnetic Transmitter](https://ieeexplore.ieee.org/document/10963877)

Yonggan Yan, Shuxiang Guo, **Bingzhi Shen**, et al., IEEE/ASME Transactions on Mechatronics, 2025

[**Project**](https://goodtime-123.github.io/projects/5dof/) <strong></strong> | [**Video**](videos/EMSensorDemo.mp4)

- Developed a 5-degrees-of-freedom electromagnetic positioning system to solve the 3D navigation challenge for interventional surgical robots
- Achieved millimeter-level dynamic tracking of miniature tools, improving accuracy by 62% over traditional methods
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><img src='images/remote.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
<div class="badge">IEEE-JSTARS (JCR Q1 IF 5.3)</div>
[DBCF-Net: Enhanced Interactive Remote Sensing Image Segmentation with a Dual-Branch Network and Collaborative Feedback Integration](https://ieeexplore.ieee.org/document/10829704)

**Bingzhi Shen**, et al., IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, 2025

[**Slide**](slide/DBCF.pdf)
- Proposed a dual-branch network with a cooperative feedback mechanism to address edge degradation and improve segmentation accuracy in complex remote sensing scenes
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/LIM.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
<div class="badge">Technical Report</div>
[Lightweight Method for Interactive 3D Medical Image Segmentation with Multi-Round Result Fusion](https://arxiv.org/pdf/2412.08315)

**Bingzhi Shen** et al., ArXiv abs/2412.08315

[**Project**](https://goodtime-123.github.io/projects/lim/) <strong></strong> | [**Video**](videos/IIS.mp4)

- Developed a lightweight interactive segmentation network (LIM-Net) and annotation system, achieving >90% DICE score on multiple datasets with a 3D inference speed of 31 FPS.

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images/MICCAI25.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
<div class="badge">MICCAI 2025 (CCF B)</div>
[Hierarchical Part-based Generative Model for Realistic 3D Blood Vessel](https://arxiv.org/pdf/2507.15223)

Siqi Chen, Guoqing Zhang, Jiahao Lai, **Bingzhi Shen**, et al., MICCAI 2025

- Developed a hierarchical part-based generative model for creating realistic 3D blood vessel structures
</div>
</div>

- [GCRNet: Global Context and Coordinate Attention-Based Double-Branch Residual Network for High Spatial Resolution Hyperspectral Image Classification](https://link.springer.com/article/10.1007/s12524-024-02083-x), **Bingzhi Shen** et al., J Indian Soc Remote Sens (2024). (JCR Q3 IF 2.2)

- [Generating Synthetic X-ray Image Methods for Vascular Interventional Surgery](https://ieeexplore.ieee.org/document/10633116), **Bingzhi Shen** et al., 2024 IEEE ICMA, Tianjin, China, 2024 (EI)


# 🎖 Honors and Awards
- *2024* Master’s Special-Grade Academic Scholarship, Beijing Institute of Technology
- *2024* National Third Prize-China Graduate Electronics Design Contest
- *2023* Outstanding Graduate, Beijing Forestry University
- *2020* National Encouragement Scholarship, Beijing Forestry University

# 📖 Educations
- *2023 - Present*, M.S. in Electronic Information (Biomedical Engineering), Beijing Institute of Technology
- *2019 - 2023*, B.S. in Electronic Information Science and Technology, Beijing Forestry University

# 🧪 Research Experience

<div class='paper-box'><div class='paper-box-text' markdown="1">
<span class="badge">LLM/NLP</span>&nbsp;**Multimodal Intelligent Public Opinion Analysis System**
![LLM-POA](/images/LLM-POA.png)
  
  - **Designed a sophisticated dual-model architecture (VLM + LLM) featuring a Divergence Arbitration Mechanism.** To enhance system reliability, I moved beyond single-model approaches. My system processes inputs with both Vision-Language and Large Language Models, then intelligently compares their outputs. In cases of disagreement, a custom-built arbitration mechanism uses expert-knowledge routing and, for highly ambiguous cases, triggers a Chain-of-Thought (CoT) re-evaluation to ensure final decision quality and robustness.
  Engineered a two-stage data synthesis pipeline to address the cold-start problem,
  - **Engineered a two-stage data synthesis pipeline to solve the cold-start problem, expanding the original dataset of 1,000 real-world business data into a high-quality training set of 10,000 samples.**. I implemented a Generate-Critique strategy, using Qwen-Max and DeepSeek-R1 for cost-effective data generation and more powerful models like GPT-4o for quality validation. Central to this was CoT Distillation—employed a teacher model to generate reasoning paths, then distilled this "think flow" into a synthetic dataset, enabling smaller fine-tuned models (7B–32B) to learn not just answers but the underlying reasoning process, thereby constructing a CoT dataset.
  - **Established a rigorous, multi-level evaluation framework focused on real-world performance and high-risk scenarios.** Beyond achieving a macro accuracy of 77.6%, I built a fine-grained evaluation system based on a 20-category confusion matrix. This allowed for the identification of specific weaknesses and the implementation of strict recall targets for critical, high-risk categories, ensuring the system met stringent safety and reliability standards.
  - **Future Research Direction**: The experience of building a robust reasoning and arbitration system has solidified my research interests. I've seen firsthand how standard SFT can fail in nuanced situations. This drives my passion to explore next-generation alignment techniques like DPO and RLHF, to build models that are not just accurate, but genuinely trustworthy and aligned with complex human preferences.

</div></div>



<div class='paper-box'><div class='paper-box-text' markdown="1">
<span class="badge">Medical Image Processing</span>&nbsp;**Real-time Stenosis Detection & Interactive Segmentation in Angiography**
![vessel](/images/vessel.gif)
<video controls width="600" height="auto">
  <source src="/images/IIS_vessel.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
  - Developed a novel loss function to improve accuracy in distinguishing between mild, moderate, and severe vascular stenosis
  - Designed a stenosis-aware attention mechanism to enhance bounding box localization and feature differentiation
  - Designed a TopoDecoder to align the Segment Anything Model (SAM) for the interactive segmentation task of angiography images
</div></div>

<div class='paper-box'><div class='paper-box-text' markdown="1">
<span class="badge">Medical Image Processing</span>&nbsp;**Interactive Medical Image Segmentation, YIZHUN AI**
  -Human-in-the-Loop AI Systems: Independently developed a lightweight interactive segmentation network (LIM-Net) and annotation system, achieving >90% DICE score on multiple datasets with a 3D inference speed of 31 FPS
  - Implemented a fusion strategy based on historical results to enhance segmentation consistency and accuracy across slices
  - Led algorithm deployment and backend development, successfully launching the system with zero-shot capabilities in several top-tier hospitals
</div></div>

<div class='paper-box'><div class='paper-box-text' markdown="1">
<span class="badge">Remote Sensing</span>&nbsp;**Interactive Segmentation for Remote Sensing Images**
  - Proposed a dual-branch network (DBCF-Net) with a cooperative feedback mechanism to address edge degradation and improve segmentation accuracy in complex remote sensing scenes
</div></div>

<div class='paper-box'><div class='paper-box-text' markdown="1">
<span class="badge">Medical Robotics</span>&nbsp;**Development of a 5-DoF Electromagnetic Positioning System for Catheter Tips**
  - Helped develop a 5-degrees-of-freedom electromagnetic positioning system to solve the 3D navigation challenge for interventional surgical robots
  - System features an innovative single-axis rotating transmitter and a CNN-LSTM model enabling millimeter-level dynamic tracking of miniature tools
  - Successfully integrated into a robot to complete navigation tasks in vascular models 
</div></div>

<div class='paper-box'><div class='paper-box-text' markdown="1">
<span class="badge">Autonomous Driving</span>&nbsp;**Novel View Synthesis Challenge for Autonomous Driving Scenarios**
  - Explored implementation of high-quality novel view synthesis for vehicle driving scenarios based on point cloud reconstruction, 3D Gaussian Splatting, and World Models
</div></div>

# 📚 Academic Service
- *2025*, Reviewer, INTERNATIONAL CONFERENCE ON MEDICAL IMAGE COMPUTING AND COMPUTER ASSISTED INTERVENTION (MICCAI, CCF B)

# 🔧 Skills
**Languages & Frameworks**: Python, PyTorch  
**LLM Research**: SFT, RLHF, ms-swift, vLLM, LLaMA-Factory, VeRL, Prompt Engineering  
**Tools**: Git, Docker, Linux, LaTeX, NVIDIA Nsight