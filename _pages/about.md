---
permalink: /
title: ""
excerpt: "Chun Xu — Junior Undergraduate @ Central South University. Research in Computer Vision and Multimodal LLMs."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<span class='anchor' id='about-me'></span>

# 👋 About Me

Hi! I'm **Chun Xu** (徐纯), a third-year undergraduate at the [School of Computer Science](http://cse.csu.edu.cn/), [Central South University](https://www.csu.edu.cn/) (CSU, "Project 985 / 211, Double First Class"), majoring in **Data Science and Big Data Technology**. I am originally from **Hefei, Anhui, China**.

My research interests lie at the intersection of **Computer Vision** and **Multimodal Large Language Models (MLLMs)**. I am especially interested in:

- **Fine-Grained Image Retrieval (FGIR)** with vision–language re-ranking
- **Parameter-Efficient Fine-Tuning** for vision foundation models (LoRA, Adapters)
- **Reinforcement Learning for Ranking** (GRPO, RLHF-style policy optimization)
- **Medical Image Analysis** with large vision foundation models

‼️ **I am currently applying for postgraduate recommendation (Tuibao 2026) and actively seeking a Master's / Ph.D. position for Fall 2027 entry. If you find my background a fit for your group, I would be very glad to hear from you.**

I currently rank **4 / 124** (Top 3.2%) in my major, with an overall GPA of **90.97 / 100**. Beyond research and coursework, I am a probationary member of the Communist Party of China, and I enjoy reading papers and exploring open-source projects on [GitHub](https://github.com/xuchun83).

📫 The fastest way to reach me is **email: [xc_anhui0@163.com](mailto:xc_anhui0@163.com)**.


# 🔥 News

- *2026.05*: 📑 Preparing application materials for **Fall 2027 graduate admission**. Open to research internships and chats.
- *2026.04*: 🎯 Our FGIR project on CUB-200 reaches **Recall@1 = 66%** (+12 points over the MS-Loss baseline) via Qwen2.5-VL + LoRA re-ranking; now integrating **GRPO** to formulate re-ranking as policy optimization.
- *2025.12*: 🏆 Awarded **National Encouragement Scholarship** by the Ministry of Education of China — *for the second time*.
- *2025.11*: 🎉 Our Provincial Undergraduate Innovation Project on **bi-eye CFP disease detection** has been concluded; a **software copyright** was registered.
- *2025.10*: 🩺 On offline evaluation, our RETFound + LoRA bi-eye model surpasses all baselines: **AUC +2.23%**, **F1 +2.82%**, and **+7.3%** accuracy on glaucoma identification.
- *2025.09*: ⛵ Released **ShipMOT**, a complex-weather maritime multi-object tracking dataset (**116,000 frames** across **550 videos**) with synthetic fog augmentation.


# 📝 Publications & Preprints

<div class="paper-box-text" markdown="1">

> Currently *in preparation*. I will update this section once our manuscripts are submitted.

If you are interested in any of the on-going projects below (FGIR re-ranking with GRPO / RETFound bi-eye CFP / ShipMOT), please feel free to **email me** for the latest draft.

</div>


# 🔬 Research Projects

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">2026 – Present</div>
      <img src='images/project-fgir.png' alt="FGIR project thumbnail" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

## Fine-Grained Image Retrieval with Multimodal Re-Ranking
*Independent research · 2026.01 – Present*

A two-stage **MS-Loss retrieval + multimodal re-ranking** FGIR framework that explores semantic–visual fusion and reinforcement-learning-based ranking optimization.

- Reproduced the **MS-Loss baseline** on CUB-200 from scratch; designed an end-to-end **Top-K re-ranking** pipeline.
- Built a **pairwise ranking model** based on **Qwen2.5-VL + LoRA**; mined hard negatives and analyzed the contribution of visual + semantic feature fusion.
- Reformulated the ranking task as a policy optimization problem via **GRPO**, transitioning from supervised pairwise learning to reward-based reinforcement learning.
- **Result: Recall@1 improved from 54% → 66%** on CUB-200.

`PyTorch` · `Qwen2.5-VL` · `LoRA` · `GRPO / RL` · `Hard Negative Mining`

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Concluded 2025</div>
      <img src='images/project-retfound.png' alt="RETFound project thumbnail" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

## Bi-Eye CFP Disease Detection with Vision Foundation Models
*Provincial Undergraduate Innovation Project (Principal Investigator)*

An **8-class multi-label** ophthalmic disease detector built on **RETFound** with a bi-eye feature-fusion module, deployed as a three-role (patient / doctor / admin) web system.

- Batch-processed ~**10,000 CFP images**; replaced fixed-parameter illumination correction with **locally-adaptive estimation** to address severe lighting variance and overexposure.
- Froze the RETFound backbone and inserted **LoRA + dual-path expert Adapters** into the first 12 layers, keeping trainable parameters **< 2%**.
- Tackled single-GPU memory limits via **gradient checkpointing + FP16 mixed-precision training**.
- **Result: +2.23% AUC, +2.82% F1** over all baselines; **+7.3%** accuracy on glaucoma. Concluded provincially; **software copyright registered**.

`RETFound` · `LoRA` · `Adapters` · `Mixed Precision` · `Medical Imaging`

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Dataset · 2025</div>
      <img src='images/project-shipmot.png' alt="ShipMOT project thumbnail" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

## ShipMOT: Multi-Object Ship Tracking under Adverse Weather
*Dataset construction & benchmark evaluation · 2025*

A maritime multi-object tracking dataset of **116,000 frames** across **550 videos**, augmented with synthetic adverse weather for robustness benchmarking.

- Constructed an **IoU-based** semi-automatic MOT annotation pipeline.
- Simulated complex weather using **MiDaS** depth estimation + an atmospheric scattering model, with **30% fog augmentation**.
- Evaluated the state-of-the-art **MOTIP** tracker; analyzed performance degradation under domain shift.
- Used **Qwen-VL** to auto-generate sequence-level semantic descriptions for multimodal analysis.

`MiDaS` · `MOTIP` · `Qwen-VL` · `Domain Augmentation` · `MOT Benchmark`

  </div>
</div>


# 📖 Education

- *2023.09 – 2027.06 (expected)*: **B.Eng. in Data Science and Big Data Technology**, [School of Computer Science](http://cse.csu.edu.cn/), **Central South University** (Project 985 & 211, "Double First Class"), Changsha, China.
  - **Major Rank: 4 / 124 (Top 3.2%)** &nbsp;·&nbsp; **GPA: 90.97 / 100**
  - **English: CET-4 (569) · CET-6 (520)**
  - **Selected coursework with scores:** Linear Algebra (**100**), Calculus (**99**), Data Structures (**95**), Algorithm Design and Analysis (**93**), Database Systems (**93**), Object-Oriented Programming in Java (**90**), Machine Learning (**88**).


# 🎖 Honors and Awards

- *2025*: **National Encouragement Scholarship** — Ministry of Education of China *(awarded for the 2nd time)*.
- *2024*: **National Encouragement Scholarship** — Ministry of Education of China.
- *2025*: **First-Class Academic Scholarship**, Central South University *(2nd time)*.
- *2024*: **First-Class Academic Scholarship**, Central South University.
- *2025*: **Provincial Undergraduate Innovation Project** — Concluded with **Software Copyright** registration.
- *2024*: **National E-Commerce Challenge** — University Second Prize.


# 🛠️ Skills

- **Programming:** Python (proficient), C++, Java
- **Deep Learning:** PyTorch, HuggingFace Transformers, training & fine-tuning
- **Vision & Multimodal:** Qwen2.5-VL, CLIP, RETFound, MiDaS
- **Parameter-Efficient Tuning:** LoRA, PEFT, Adapter Tuning
- **Training Tricks:** Mixed Precision (FP16), Gradient Checkpointing, Hard Negative Mining
- **Tools:** Git / GitHub, Linux, VS Code / Cursor, LaTeX
- **Languages:** Mandarin (native), English (CET-6 / 520)


# 📫 Contact

- 📧 Email: <a href="mailto:xc_anhui0@163.com">xc_anhui0@163.com</a>
- 💻 GitHub: [github.com/xuchun83](https://github.com/xuchun83)
- 📍 Based in Changsha, Hunan (school) · Originally from Hefei, Anhui

<br/>

<p style="text-align:center; color:#888; font-size:0.9em;">
  Last updated: 2026 · Built with <a href="https://github.com/RayeRen/acad-homepage.github.io">acad-homepage</a> · Hosted on GitHub Pages
</p>
