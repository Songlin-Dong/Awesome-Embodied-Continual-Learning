# Awesome Embodied Continual Learning [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of papers and resources on **Embodied Continual Learning** — the intersection of continual/lifelong learning and embodied intelligence, covering manipulation, navigation, whole-body control, VLA models, and more.

Maintained by [Songlin Dong (董松林)](https://songlin-dong.github.io) @ SUAT. Contributions welcome — please read [CONTRIBUTING.md](CONTRIBUTING.md) and submit a pull request!

If you find this repository helpful, please consider giving it a ⭐.

> **⚠️ CL Verification Note:** Papers marked with ⚠️ are included for reference but are *on the boundary* of continual learning (e.g., skill discovery, few-shot adaptation, or multi-task learning without explicit modeling of catastrophic forgetting or sequential task learning). We include them for completeness and leave community discussion open via Issues.

---

## 📌 Table of Contents

- [What is Embodied Continual Learning?](#what-is-embodied-continual-learning)
- [Survey & Overview](#survey--overview)
- [By Embodied Task](#by-embodied-task)
  - [Manipulation](#-manipulation)
  - [Navigation](#-navigation)
  - [Whole-Body Control & Locomotion](#-whole-body-control--locomotion)
  - [Multi-Task & General Embodied Agent](#-multi-task--general-embodied-agent)
  - [Scene Understanding & Perception](#-scene-understanding--perception)
  - [Instruction Following & Vision-Language](#-instruction-following--vision-language)
- [Vision-Language-Action (VLA) Continual Learning](#vision-language-action-vla-continual-learning)
- [By Continual Learning Approach](#by-continual-learning-approach)
  - [Continual Imitation Learning](#continual-imitation-learning)
  - [Continual Reinforcement Learning](#continual-reinforcement-learning)
  - [Replay-Based Methods](#replay-based-methods)
  - [Regularization-Based Methods](#regularization-based-methods)
  - [Architecture-Based Methods](#architecture-based-methods)
  - [Prompt / Parameter-Efficient Methods](#prompt--parameter-efficient-methods)
- [By Year](#by-year)
  - [2026](#2026)
  - [2025](#2025)
  - [2024](#2024)
  - [2023](#2023)
  - [2022 and Before](#2022-and-before)
- [Benchmarks & Datasets](#benchmarks--datasets)
- [Related Awesome Lists](#related-awesome-lists)

---

## What is Embodied Continual Learning?

**Embodied Continual Learning (ECL)** studies how embodied agents (robots, virtual avatars, autonomous systems) can continuously acquire new skills and adapt to new environments **without forgetting previously learned ones**. It sits at the intersection of:

- 🤖 **Embodied AI** — agents that perceive, reason, and act in physical or simulated worlds
- 🔄 **Continual / Lifelong Learning** — learning sequentially without catastrophic forgetting
- 🧠 **Skill Transfer** — reusing and composing learned skills across tasks and domains

Key challenges include: non-stationary environments, partial observability, action-space expansion, and the high cost of robot experience collection.

---

## Survey & Overview

- A Survey of Continual Reinforcement Learning (arXiv2024) [[paper](https://arxiv.org/abs/2408.09893)]
- Towards Continual Reinforcement Learning: A Review and Perspectives (arXiv2020) [[paper](https://arxiv.org/abs/2012.13490)]
- Continual Learning in Robotics: Definition, Framework, Learning Strategies, Opportunities and Challenges (Neural Networks 2022) [[paper](https://doi.org/10.1016/j.neunet.2022.02.016)]
- A Comprehensive Survey of Continual Learning: Theory, Method and Application (TPAMI2024) [[paper](https://arxiv.org/abs/2302.00487)]

---

## By Embodied Task

### 🦾 Manipulation

> Papers on robots continuously learning to grasp, assemble, pour, or otherwise manipulate objects across tasks.

- Think Small, Act Big: Primitive Prompt Learning for Lifelong Robot Manipulation (CVPR2025) [[paper](https://arxiv.org/abs/2504.00420)]
- iManip: Skill-Incremental Learning for Robotic Manipulation (ICCV2025) [[paper](https://arxiv.org/abs/2503.07087)]
- Few-Shot Vision-Language Action-Incremental Policy Learning (arXiv2025) [[paper](https://arxiv.org/abs/2504.15517)]
- SPECI: Skill Prompts based Hierarchical Continual Imitation Learning for Robot Manipulation (arXiv2025) [[paper](https://arxiv.org/abs/2504.15561)]
- M2Distill: Multi-Modal Distillation for Lifelong Imitation Learning (ICRA2025) [[paper](https://arxiv.org/abs/2410.00064)]
- Dynamic Mixture of Progressive Parameter-Efficient Expert Library for Lifelong Robot Learning (arXiv2024) [[paper](https://arxiv.org/abs/2408.11430)]
- TAIL: Task-specific Adapters for Imitation Learning with Large Pretrained Models (ICLR2024) [[paper](https://arxiv.org/abs/2310.05905)]
- Never-Ending Behavior-Cloning Agent for Robotic Manipulation (CoRL2023) [[paper](https://arxiv.org/abs/2304.04395)]
- CRIL: Continual Robot Imitation Learning via Generative and Prediction Model (IROS2021) [[paper](https://arxiv.org/abs/2106.09422)] [[code](https://github.com/HeegerGao/CRIL)]
- Experience Consistency Distillation Continual RL for Robotic Manipulation Tasks (arXiv2024) [[paper](https://arxiv.org/abs/2410.01373)]
- Continual Policy Distillation of RL-based Controllers for Soft Robotic In-Hand Manipulation (IROS2023) [[paper](https://arxiv.org/abs/2309.07898)]
- Forgetting and Imbalance in Robot Lifelong Learning with Off-policy Data (arXiv2024) [[paper](https://arxiv.org/abs/2404.07048)]
- Lifelong Robotic Reinforcement Learning by Retaining Experiences (arXiv2021) [[paper](https://arxiv.org/abs/2109.09180)]
- AutoCGP: Closed-Loop Concept-Guided Policies from Unlabeled Demonstrations (ICLR2025) ⚠️ [[paper](https://openreview.net/forum?id=9ehJCZz4aM)] [[code](https://github.com/PeiZhou26/AutoCGP)]
- Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation (RAL2022) ⚠️ [[paper](https://arxiv.org/abs/2109.13779)]
- Composing Diffusion Policies for Few-Shot Learning of Movement Trajectories (arXiv2023) ⚠️ [[paper](https://arxiv.org/abs/2311.06534)]
- Coupled Distributional Random Expert Distillation for World Model Online Imitation Learning (arXiv2024) ⚠️ [[paper](https://arxiv.org/abs/2401.09935)]

---

### 🧭 Navigation

> Papers on agents continuously learning to navigate in new environments, with new goals or layouts, without forgetting prior routes.

- Trajectory-Diversity-Driven Robust Vision-and-Language Navigation (CVPR2026 Finding) [[paper](#)] — *Corresponding: Songlin Dong*
- Learning to Navigate for Mobile Robot with Continual Reinforcement Learning (IROS2021) [[paper](https://arxiv.org/abs/2110.04991)]
- Evaluating Continual Learning on a Home Robot (arXiv2022) [[paper](https://arxiv.org/abs/2205.04020)]

---

### 🏃 Whole-Body Control & Locomotion

> Papers on legged robots or full-body agents that incrementally learn new gaits, terrains, or motor skills.

*Papers coming soon — submit a PR!*

---

### 🌐 Multi-Task & General Embodied Agent

> Papers on general embodied agents that learn heterogeneous tasks continually.

- Hierarchical-Task-Aware Multi-modal Mixture of Incremental LoRA Experts for Embodied Continual Learning (ACL2025) [[paper](https://aclanthology.org/2025.acl-long.1379/)] [[arxiv](https://arxiv.org/abs/2506.04595)]
- Behavior Self-Organization Supports Task Inference for Continual Robot Learning (IROS2023) [[paper](https://arxiv.org/abs/2309.16245)]
- Modular Lifelong Reinforcement Learning via Neural Composition (ICLR2022) [[paper](https://arxiv.org/abs/2207.00429)]
- Learning Modular Neural Network Policies for Multi-Task and Multi-Robot Transfer (ICRA2017) [[paper](https://arxiv.org/abs/1609.07088)]
- Diffusion Augmented Agents: A Framework for Efficient Exploration and Transfer Learning (arXiv2023) [[paper](https://arxiv.org/abs/2310.17482)]
- A Simple Approach to Continual Learning by Transferring Skill Parameters (arXiv2023) [[paper](https://arxiv.org/abs/2304.09520)]
- Model Primitive Hierarchical Lifelong Reinforcement Learning (arXiv2022) [[paper](https://arxiv.org/abs/2209.13670)]
- PolyTask: Learning Unified Policies through Behavior Distillation (arXiv2023) ⚠️ [[paper](https://arxiv.org/abs/2310.08573)]

---

### 👁️ Scene Understanding & Perception

> Continual 3D scene understanding, object detection, segmentation, and mapping in embodied settings.

*Papers coming soon — submit a PR!*

---

### 💬 Instruction Following & Vision-Language

> Agents that incrementally follow natural-language instructions, acquire new concepts from VLMs, and generalize to new command distributions.

- Trajectory-Diversity-Driven Robust Vision-and-Language Navigation (CVPR2026 Finding) [[paper](#)] — *Corresponding: Songlin Dong*
- ReMoT: Reinforcement Learning with Motion Contrast Triplets (CVPR2026) [[paper](#)] — *Corresponding: Songlin Dong*

---

## Vision-Language-Action (VLA) Continual Learning

> Papers on continual learning for **Vision-Language-Action models** — large pre-trained VLA models (e.g. RT-2, OpenVLA, π₀, RoboFlamingo) that are incrementally fine-tuned on new tasks, objects, or environments while retaining prior capabilities. This category focuses specifically on works where the **action prediction head** is jointly trained with visual and language encoders in an end-to-end manner, distinguishing it from pure VLN or manipulation-only works.

- Hierarchical-Task-Aware Multi-modal Mixture of Incremental LoRA Experts for Embodied Continual Learning (ACL2025) [[paper](https://aclanthology.org/2025.acl-long.1379/)] [[arxiv](https://arxiv.org/abs/2506.04595)]
- Few-Shot Vision-Language Action-Incremental Policy Learning (arXiv2025) [[paper](https://arxiv.org/abs/2504.15517)]
- Think Small, Act Big: Primitive Prompt Learning for Lifelong Robot Manipulation (CVPR2025) [[paper](https://arxiv.org/abs/2504.00420)]
- iManip: Skill-Incremental Learning for Robotic Manipulation (ICCV2025) [[paper](https://arxiv.org/abs/2503.07087)]
- TAIL: Task-specific Adapters for Imitation Learning with Large Pretrained Models (ICLR2024) [[paper](https://arxiv.org/abs/2310.05905)]

---

## By Continual Learning Approach

### Continual Imitation Learning

> Methods that address catastrophic forgetting in imitation learning (behavior cloning, IRL, etc.) for embodied agents learning sequentially from expert demonstrations.

- Think Small, Act Big: Primitive Prompt Learning for Lifelong Robot Manipulation (CVPR2025) [[paper](https://arxiv.org/abs/2504.00420)]
- iManip: Skill-Incremental Learning for Robotic Manipulation (ICCV2025) [[paper](https://arxiv.org/abs/2503.07087)]
- Few-Shot Vision-Language Action-Incremental Policy Learning (arXiv2025) [[paper](https://arxiv.org/abs/2504.15517)]
- SPECI: Skill Prompts based Hierarchical Continual Imitation Learning for Robot Manipulation (arXiv2025) [[paper](https://arxiv.org/abs/2504.15561)]
- Hierarchical-Task-Aware Multi-modal Mixture of Incremental LoRA Experts for Embodied Continual Learning (ACL2025) [[paper](https://aclanthology.org/2025.acl-long.1379/)]
- M2Distill: Multi-Modal Distillation for Lifelong Imitation Learning (ICRA2025) [[paper](https://arxiv.org/abs/2410.00064)]
- Dynamic Mixture of Progressive Parameter-Efficient Expert Library for Lifelong Robot Learning (arXiv2024) [[paper](https://arxiv.org/abs/2408.11430)]
- TAIL: Task-specific Adapters for Imitation Learning with Large Pretrained Models (ICLR2024) [[paper](https://arxiv.org/abs/2310.05905)]
- Never-Ending Behavior-Cloning Agent for Robotic Manipulation (CoRL2023) [[paper](https://arxiv.org/abs/2304.04395)]
- Fast Lifelong Adaptive Inverse Reinforcement Learning from Demonstrations (CoRL2022) [[paper](https://arxiv.org/abs/2209.11908)]
- CRIL: Continual Robot Imitation Learning via Generative and Prediction Model (IROS2021) [[paper](https://arxiv.org/abs/2106.09422)] [[code](https://github.com/HeegerGao/CRIL)]

---

### Continual Reinforcement Learning

> Methods that address sequential task learning and catastrophic forgetting in RL for embodied agents.

- A Definition of Continual Reinforcement Learning (NeurIPS2023) [[paper](https://arxiv.org/abs/2307.11046)]
- Continual Reinforcement Learning by Planning with Online World Models (ICML2025) [[paper](https://arxiv.org/abs/2402.12908)]
- CoMPS: Continual Meta Policy Search (arXiv2022) [[paper](https://arxiv.org/abs/2112.04467)]
- Task-Agnostic Continual Reinforcement Learning: Gaining Insights and Overcoming Challenges (CoLLAs2023) [[paper](https://arxiv.org/abs/2205.14495)]
- Building a Subspace of Policies for Scalable Continual Reinforcement Learning (ICLR2023) [[paper](https://arxiv.org/abs/2211.10445)]
- Behavior Self-Organization Supports Task Inference for Continual Robot Learning (IROS2023) [[paper](https://arxiv.org/abs/2309.16245)]
- Self-Composing Policies for Scalable Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2207.02631)]
- Modular Lifelong Reinforcement Learning via Neural Composition (ICLR2022) [[paper](https://arxiv.org/abs/2207.00429)]
- Self-Activating Neural Ensembles for Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2309.08986)]
- Continual Vision-based Reinforcement Learning with Group Symmetries (CoRL2023) [[paper](https://arxiv.org/abs/2310.11436)]
- Continual Model-Based Reinforcement Learning with Hypernetworks (ICRA2021) [[paper](https://arxiv.org/abs/2009.11997)]
- Continual Policy Distillation of RL-based Controllers for Soft Robotic In-Hand Manipulation (IROS2023) [[paper](https://arxiv.org/abs/2309.07898)]
- DisCoRL: Continual Reinforcement Learning via Policy Distillation (arXiv2019) [[paper](https://arxiv.org/abs/1907.05855)]
- Continual Reinforcement Learning deployed in Real-life using Policy Distillation and Sim2Real Transfer (IROS2021) [[paper](https://arxiv.org/abs/2111.04067)]
- Disentangling Transfer in Continual Reinforcement Learning (arXiv2022) [[paper](https://arxiv.org/abs/2209.13900)]
- Model Primitive Hierarchical Lifelong Reinforcement Learning (arXiv2022) [[paper](https://arxiv.org/abs/2209.13670)]
- Lifelong Robotic Reinforcement Learning by Retaining Experiences (arXiv2021) [[paper](https://arxiv.org/abs/2109.09180)]
- Deep Reinforcement Learning amidst Lifelong Non-Stationarity (ICML2021) [[paper](https://arxiv.org/abs/2006.10701)]
- A Simple Approach to Continual Learning by Transferring Skill Parameters (arXiv2023) [[paper](https://arxiv.org/abs/2304.09520)]
- Replay-Enhanced Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2311.11557)]
- Learning an Embedding Space for Transferable Robot Skills (ICLR2018) [[paper](https://openreview.net/forum?id=rk07ZXZRb)]
- Learning to Navigate for Mobile Robot with Continual Reinforcement Learning (IROS2021) [[paper](https://arxiv.org/abs/2110.04991)]
- Forgetting and Imbalance in Robot Lifelong Learning with Off-policy Data (arXiv2024) [[paper](https://arxiv.org/abs/2404.07048)]
- Experience Consistency Distillation Continual RL for Robotic Manipulation Tasks (arXiv2024) [[paper](https://arxiv.org/abs/2410.01373)]
- Diffusion Augmented Agents: A Framework for Efficient Exploration and Transfer Learning (arXiv2023) [[paper](https://arxiv.org/abs/2310.17482)]
- Learning Modular Neural Network Policies for Multi-Task and Multi-Robot Transfer (ICRA2017) [[paper](https://arxiv.org/abs/1609.07088)]
- Evaluating Continual Learning on a Home Robot (arXiv2022) [[paper](https://arxiv.org/abs/2205.04020)]
- Robust RL in Continuous Control Tasks with Uncertainty Set Regularization (arXiv2022) ⚠️ [[paper](https://arxiv.org/abs/2207.02038)]

---

### Replay-Based Methods

- CRIL: Continual Robot Imitation Learning via Generative and Prediction Model (IROS2021) [[paper](https://arxiv.org/abs/2106.09422)] [[code](https://github.com/HeegerGao/CRIL)]
- Replay-Enhanced Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2311.11557)]
- Experience Consistency Distillation Continual RL for Robotic Manipulation Tasks (arXiv2024) [[paper](https://arxiv.org/abs/2410.01373)]
- M2Distill: Multi-Modal Distillation for Lifelong Imitation Learning (ICRA2025) [[paper](https://arxiv.org/abs/2410.00064)]
- Lifelong Robotic Reinforcement Learning by Retaining Experiences (arXiv2021) [[paper](https://arxiv.org/abs/2109.09180)]

---

### Regularization-Based Methods

- Continual Model-Based Reinforcement Learning with Hypernetworks (ICRA2021) [[paper](https://arxiv.org/abs/2009.11997)]
- Deep Reinforcement Learning amidst Lifelong Non-Stationarity (ICML2021) [[paper](https://arxiv.org/abs/2006.10701)]
- M2Distill: Multi-Modal Distillation for Lifelong Imitation Learning (ICRA2025) [[paper](https://arxiv.org/abs/2410.00064)]

---

### Architecture-Based Methods

- Is Parameter Isolation Better for Prompt-Based Continual Learning? (CVPR2026) [[paper](https://arxiv.org/abs/2601.20894)]
- Building a Subspace of Policies for Scalable Continual Reinforcement Learning (ICLR2023) [[paper](https://arxiv.org/abs/2211.10445)]
- Self-Composing Policies for Scalable Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2207.02631)]
- Modular Lifelong Reinforcement Learning via Neural Composition (ICLR2022) [[paper](https://arxiv.org/abs/2207.00429)]
- Self-Activating Neural Ensembles for Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2309.08986)]
- Dynamic Mixture of Progressive Parameter-Efficient Expert Library for Lifelong Robot Learning (arXiv2024) [[paper](https://arxiv.org/abs/2408.11430)]

---

### Prompt / Parameter-Efficient Methods

- Is Parameter Isolation Better for Prompt-Based Continual Learning? (CVPR2026) [[paper](https://arxiv.org/abs/2601.20894)]
- Shared & Domain Self-Adaptive Experts with Frequency-Aware Discrimination for Continual Test-Time Adaptation (AAAI2026) [[paper](#)]
- Think Small, Act Big: Primitive Prompt Learning for Lifelong Robot Manipulation (CVPR2025) [[paper](https://arxiv.org/abs/2504.00420)]
- Hierarchical-Task-Aware Multi-modal Mixture of Incremental LoRA Experts for Embodied Continual Learning (ACL2025) [[paper](https://aclanthology.org/2025.acl-long.1379/)]
- SPECI: Skill Prompts based Hierarchical Continual Imitation Learning for Robot Manipulation (arXiv2025) [[paper](https://arxiv.org/abs/2504.15561)]
- iManip: Skill-Incremental Learning for Robotic Manipulation (ICCV2025) [[paper](https://arxiv.org/abs/2503.07087)]
- TAIL: Task-specific Adapters for Imitation Learning with Large Pretrained Models (ICLR2024) [[paper](https://arxiv.org/abs/2310.05905)]
- CoMPS: Continual Meta Policy Search (arXiv2022) [[paper](https://arxiv.org/abs/2112.04467)]

---

## By Year

### 2026

- Is Parameter Isolation Better for Prompt-Based Continual Learning? (CVPR2026) [[paper](https://arxiv.org/abs/2601.20894)]
- ReMoT: Reinforcement Learning with Motion Contrast Triplets (CVPR2026) [[paper](#)] — *Corresponding: Songlin Dong*
- Trajectory-Diversity-Driven Robust Vision-and-Language Navigation (CVPR2026 Finding) [[paper](#)] — *Corresponding: Songlin Dong*
- Shared & Domain Self-Adaptive Experts with Frequency-Aware Discrimination for Continual Test-Time Adaptation (AAAI2026) [[paper](#)]

---

### 2025

- Think Small, Act Big: Primitive Prompt Learning for Lifelong Robot Manipulation (CVPR2025) [[paper](https://arxiv.org/abs/2504.00420)]
- iManip: Skill-Incremental Learning for Robotic Manipulation (ICCV2025) [[paper](https://arxiv.org/abs/2503.07087)]
- Hierarchical-Task-Aware Multi-modal Mixture of Incremental LoRA Experts for Embodied Continual Learning (ACL2025) [[paper](https://aclanthology.org/2025.acl-long.1379/)] [[arxiv](https://arxiv.org/abs/2506.04595)]
- Few-Shot Vision-Language Action-Incremental Policy Learning (arXiv2025) [[paper](https://arxiv.org/abs/2504.15517)]
- SPECI: Skill Prompts based Hierarchical Continual Imitation Learning for Robot Manipulation (arXiv2025) [[paper](https://arxiv.org/abs/2504.15561)]
- M2Distill: Multi-Modal Distillation for Lifelong Imitation Learning (ICRA2025) [[paper](https://arxiv.org/abs/2410.00064)]
- Continual Reinforcement Learning by Planning with Online World Models (ICML2025) [[paper](https://arxiv.org/abs/2402.12908)]
- AutoCGP: Closed-Loop Concept-Guided Policies from Unlabeled Demonstrations (ICLR2025) ⚠️ [[paper](https://openreview.net/forum?id=9ehJCZz4aM)] [[code](https://github.com/PeiZhou26/AutoCGP)]

---

### 2024

- Dynamic Mixture of Progressive Parameter-Efficient Expert Library for Lifelong Robot Learning (arXiv2024) [[paper](https://arxiv.org/abs/2408.11430)]
- TAIL: Task-specific Adapters for Imitation Learning with Large Pretrained Models (ICLR2024) [[paper](https://arxiv.org/abs/2310.05905)]
- A Survey of Continual Reinforcement Learning (arXiv2024) [[paper](https://arxiv.org/abs/2408.09893)]
- Forgetting and Imbalance in Robot Lifelong Learning with Off-policy Data (arXiv2024) [[paper](https://arxiv.org/abs/2404.07048)]
- Experience Consistency Distillation Continual RL for Robotic Manipulation Tasks (arXiv2024) [[paper](https://arxiv.org/abs/2410.01373)]
- Coupled Distributional Random Expert Distillation for World Model Online Imitation Learning (arXiv2024) ⚠️ [[paper](https://arxiv.org/abs/2401.09935)]

---

### 2023

- A Definition of Continual Reinforcement Learning (NeurIPS2023) [[paper](https://arxiv.org/abs/2307.11046)]
- Building a Subspace of Policies for Scalable Continual Reinforcement Learning (ICLR2023) [[paper](https://arxiv.org/abs/2211.10445)]
- Behavior Self-Organization Supports Task Inference for Continual Robot Learning (IROS2023) [[paper](https://arxiv.org/abs/2309.16245)]
- Self-Composing Policies for Scalable Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2207.02631)]
- Self-Activating Neural Ensembles for Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2309.08986)]
- Continual Vision-based Reinforcement Learning with Group Symmetries (CoRL2023) [[paper](https://arxiv.org/abs/2310.11436)]
- Continual Policy Distillation of RL-based Controllers for Soft Robotic In-Hand Manipulation (IROS2023) [[paper](https://arxiv.org/abs/2309.07898)]
- Task-Agnostic Continual Reinforcement Learning: Gaining Insights and Overcoming Challenges (CoLLAs2023) [[paper](https://arxiv.org/abs/2205.14495)]
- Never-Ending Behavior-Cloning Agent for Robotic Manipulation (CoRL2023) [[paper](https://arxiv.org/abs/2304.04395)]
- LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning (NeurIPS2023) [[paper](https://arxiv.org/abs/2306.03310)] [[code](https://github.com/Lifelong-Robot-Learning/LIBERO)]
- Replay-Enhanced Continual Reinforcement Learning (arXiv2023) [[paper](https://arxiv.org/abs/2311.11557)]
- Diffusion Augmented Agents: A Framework for Efficient Exploration and Transfer Learning (arXiv2023) [[paper](https://arxiv.org/abs/2310.17482)]
- A Simple Approach to Continual Learning by Transferring Skill Parameters (arXiv2023) [[paper](https://arxiv.org/abs/2304.09520)]
- Composing Diffusion Policies for Few-Shot Learning of Movement Trajectories (arXiv2023) ⚠️ [[paper](https://arxiv.org/abs/2311.06534)]
- PolyTask: Learning Unified Policies through Behavior Distillation (arXiv2023) ⚠️ [[paper](https://arxiv.org/abs/2310.08573)]

---

### 2022 and Before

- Fast Lifelong Adaptive Inverse Reinforcement Learning from Demonstrations (CoRL2022) [[paper](https://arxiv.org/abs/2209.11908)]
- Modular Lifelong Reinforcement Learning via Neural Composition (ICLR2022) [[paper](https://arxiv.org/abs/2207.00429)]
- Disentangling Transfer in Continual Reinforcement Learning (arXiv2022) [[paper](https://arxiv.org/abs/2209.13900)]
- Model Primitive Hierarchical Lifelong Reinforcement Learning (arXiv2022) [[paper](https://arxiv.org/abs/2209.13670)]
- Evaluating Continual Learning on a Home Robot (arXiv2022) [[paper](https://arxiv.org/abs/2205.04020)]
- CoMPS: Continual Meta Policy Search (arXiv2022) [[paper](https://arxiv.org/abs/2112.04467)]
- Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation (RAL2022) ⚠️ [[paper](https://arxiv.org/abs/2109.13779)]
- Continual Model-Based Reinforcement Learning with Hypernetworks (ICRA2021) [[paper](https://arxiv.org/abs/2009.11997)]
- CRIL: Continual Robot Imitation Learning via Generative and Prediction Model (IROS2021) [[paper](https://arxiv.org/abs/2106.09422)] [[code](https://github.com/HeegerGao/CRIL)]
- Continual Reinforcement Learning deployed in Real-life using Policy Distillation and Sim2Real Transfer (IROS2021) [[paper](https://arxiv.org/abs/2111.04067)]
- Deep Reinforcement Learning amidst Lifelong Non-Stationarity (ICML2021) [[paper](https://arxiv.org/abs/2006.10701)]
- Lifelong Robotic Reinforcement Learning by Retaining Experiences (arXiv2021) [[paper](https://arxiv.org/abs/2109.09180)]
- Learning to Navigate for Mobile Robot with Continual Reinforcement Learning (IROS2021) [[paper](https://arxiv.org/abs/2110.04991)]
- Continual World: A Robotic Benchmark for Continual Reinforcement Learning (NeurIPS2021) [[paper](https://arxiv.org/abs/2105.10919)] [[code](https://github.com/awarelab/continual_world)]
- DisCoRL: Continual Reinforcement Learning via Policy Distillation (arXiv2019) [[paper](https://arxiv.org/abs/1907.05855)]
- Learning an Embedding Space for Transferable Robot Skills (ICLR2018) [[paper](https://openreview.net/forum?id=rk07ZXZRb)]
- Learning Modular Neural Network Policies for Multi-Task and Multi-Robot Transfer (ICRA2017) [[paper](https://arxiv.org/abs/1609.07088)]

---

## Benchmarks & Datasets

| Name | Task | Year | Paper | Code |
|------|------|------|-------|------|
| **LIBERO** | Manipulation (lifelong IL) | NeurIPS2023 | [paper](https://arxiv.org/abs/2306.03310) | [code](https://github.com/Lifelong-Robot-Learning/LIBERO) |
| **Continual World** | Manipulation (CRL, Meta-World) | NeurIPS2021 | [paper](https://arxiv.org/abs/2105.10919) | [code](https://github.com/awarelab/continual_world) |
| **CORA** | General CRL benchmark | arXiv2022 | [paper](https://arxiv.org/abs/2110.10067) | [code](https://github.com/AGI-Labs/continual_rl) |
| **RLBench** | Manipulation | RAL2020 | [paper](https://arxiv.org/abs/1909.12271) | [code](https://github.com/stepjam/RLBench) |
| **Habitat** | Navigation | ICCV2019 | [paper](https://arxiv.org/abs/1904.01201) | [code](https://github.com/facebookresearch/habitat-sim) |
| **iGibson** | Navigation + Manipulation | RAL2021 | [paper](https://arxiv.org/abs/2012.02924) | [code](https://github.com/StanfordVL/iGibson) |
| **BEHAVIOR** | Household Activities | NeurIPS2021 | [paper](https://arxiv.org/abs/2108.03332) | [code](https://github.com/StanfordVL/behavior) |
| **Procgen** | Generalization / Non-stationarity | ICML2020 | [paper](https://arxiv.org/abs/1912.01588) | [code](https://github.com/openai/procgen) |

---

## Related Awesome Lists

- [Awesome Incremental Learning](https://github.com/xialeiliu/Awesome-Incremental-Learning) — General continual/incremental learning
- [Awesome Continual Learning](https://github.com/optimass/continual_learning_papers) — Broad continual learning papers
- [Awesome Embodied AI (VLA/VLN)](https://github.com/jonyzhang2023/awesome-embodied-vla-va-vln) — VLA, VLN and embodied AI
- [Awesome Robot Learning](https://github.com/jsxzs/Awesome-Robot-Learning) — Robot learning papers
- [Awesome Vision-Language Navigation](https://github.com/daqingliu/awesome-vln) — VLN papers

---

## Contributing

Please see [CONTRIBUTING.md](CONTRIBUTING.md). Format for each entry:
```
Paper Title (VenueYear) [[paper](url)] [[code](url)]
```

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Songlin Dong](https://songlin-dong.github.io) has waived all copyright and related rights to this work.

---

<p align="center">
  <i>Last updated: March 2026 · Maintained by <a href="https://songlin-dong.github.io">Songlin Dong</a></i>
</p>
