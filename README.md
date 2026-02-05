# HoRD: Robust Humanoid Control via History-Conditioned Reinforcement Learning and Online Distillation

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/tonywang-0517/hord)
[![Project](https://img.shields.io/badge/Project-Page-green)](https://tonywang-0517.github.io/hord/)

Project page for **HoRD: Robust Humanoid Control via History-Conditioned Reinforcement Learning and Online Distillation** by Puyue Wang, Jiawei Hu, Yan Gao, Junyan Wang, Yu Zhang, Gillian Dobbie, Tao Gu, Wafa Johal, Ting Dang, Hong Jia (2026).

A two-stage learning framework for robust humanoid control under domain shift, achieving substantially higher success rates under domain shifts and enabling reliable zero-shot sim-to-sim transfer to unseen physics engines.

## Overview

Humanoid robots can suffer significant performance drops under small changes in dynamics, task specifications, or environment setup. HoRD introduces two key components:

- **SSJR** (Standardized Sparse-Joint Representation): A standardized sparse-joint protocol that unifies fragmented motion sources into a platform-agnostic sparse-joint command interface
- **HCDR** (History-Conditioned Dynamics Representation): A history-conditioned representation module that encodes recent state–action history into a temporal memory embedding for online dynamics inference and adaptive modulation

## Key Results

- **90.7%** success rate in training simulator (IsaacLab)
- **86.0%** success rate in zero-shot transfer to unseen physics engine (Genesis)
- Significantly outperforms strong baselines including MaskedMimic, OmniH2O, ExBody2, and Hover
- Robust performance across six representative motions under zero-shot domain transfer

## Links

- **Project Page**: [https://tonywang-0517.github.io/hord/](https://tonywang-0517.github.io/hord/)
- **GitHub Repository**: [https://github.com/tonywang-0517/hord](https://github.com/tonywang-0517/hord)
- **Paper**: [arXiv:2602.04412](https://arxiv.org/abs/2602.04412)
- **Video**: [YouTube](https://www.youtube.com/watch?v=YOUR_VIDEO_ID) (Coming soon)

## Project Structure

```
hord/
├── index.html              # Main project page
├── static/
│   ├── css/               # Stylesheets
│   │   └── index.css      # Main stylesheet with sand/gold theme variables
│   ├── js/                # JavaScript files
│   ├── images/            # Images and visualizations
│   │   ├── bg.png                      # Hero section background
│   │   ├── hord_overview.png           # Framework overview
│   │   ├── teacher_training_stage1.jpg # Training stage 1
│   │   ├── student_training_stage2.jpg # Training stage 2
│   │   ├── hord_eval_process.jpg       # Evaluation process
│   │   ├── method_comparison.png       # Ablation training curves
│   │   ├── metrics_comparison.png      # Training metrics comparison
│   │   ├── all_metrics_eval_combined.png # Ablation results on Genesis
│   │   ├── terrain.png                 # Terrain diversity
│   │   └── favicon.ico                 # Site favicon
│   └── videos/            # Demo videos
│       ├── eval/           # Evaluation videos
│       │   ├── 1_punch/hord/tmp_video.mp4
│       │   ├── 2_getup/hord/tmp_video.mp4
│       │   ├── 3_high_kick/hord/tmp_video.mp4
│       │   ├── 4_common_walk/hord/tmp_video.mp4
│       │   ├── 5_side_walk/hord/tmp_video.mp4
│       │   └── 6_martial/hord/tmp_video.mp4
│       ├── g1_random_push.mp4          # Random perturbation recovery
│       ├── masked_mimic_g1_no_vae.mp4  # Teacher-student distillation
│       └── ...
└── README.md              # This file
```

## Features

- **Hero Section**: Eye-catching introduction with custom background image
- **Performance Highlights**: Interactive cards showcasing key success rates
- **Two Core Components**: Detailed explanation of SSJR and HCDR
- **Training Methodology**: Two-stage teacher-student training architecture with domain randomization
- **Sim-to-Sim Transfer Performance**: Comprehensive comparison table with baselines
- **Ablation Studies**: Component analysis, training curves, and test results
- **Representative Motion Demonstrations**: Six motion videos under zero-shot domain transfer
- **Policy Structure Comparison**: Method comparison table
- **Live Demonstrations**: Robust recovery and expert distillation videos
- **Terrain Diversity**: Analysis across varied environmental conditions

## Citation

```bibtex
@article{wang2026hord,
  title={HoRD: Robust Humanoid Control via History-Conditioned Reinforcement Learning and Online Distillation},
  author={Wang, Puyue and Hu, Jiawei and Gao, Yan and Wang, Junyan and Zhang, Yu and Dobbie, Gillian and Gu, Tao and Johal, Wafa and Dang, Ting and Jia, Hong},
  year={2026},
  journal={Preprint},
  url={https://github.com/tonywang-0517/hord}
}
```

## Development

The project page uses modern web technologies:
- **Bulma CSS** framework for responsive design
- **Font Awesome** for icons
- **Bulma Carousel** for image/video carousels
- **Custom CSS variables** for sand/gold theme consistency
- **CSS gradient styles** for visual appeal
- Optimized for performance and SEO

### Theme Colors

The page uses a sand/gold color theme defined in CSS variables:
- Primary color: `#e8c99b` (light sand gold)
- Primary hover: `#d4a574` (medium sand gold)
- Primary dark: `#b8864a` (dark sand gold)
- All colors are centrally managed through CSS variables in `static/css/index.css`

## Media Assets

### Images
All images are properly referenced and positioned:
- `bg.png` - Hero section background image
- `hord_overview.png` - Framework overview diagram
- `teacher_training_stage1.jpg` - Stage 1 training visualization
- `student_training_stage2.jpg` - Stage 2 training visualization
- `hord_eval_process.jpg` - Evaluation methodology visualization
- `method_comparison.png` - Ablation training curves comparison
- `metrics_comparison.png` - Training metrics comparison
- `all_metrics_eval_combined.png` - Ablation results on Genesis test dataset
- `terrain.png` - Terrain diversity analysis

### Videos
- **Evaluation Videos**: Six representative motions (punch, get up, high kick, common walk, side walk, martial) under zero-shot domain transfer
- `g1_random_push.mp4` - Random perturbation recovery demonstration
- `masked_mimic_g1_no_vae.mp4` - Teacher-student distillation demonstration

## Website License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
