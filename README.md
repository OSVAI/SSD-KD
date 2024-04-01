# Small Scale Data-Free Knowledge Distillation (SSD-KD)

By He Liu, Yikai Wang, Huaping Liu, Fuchun Sun and Anbang Yao

This repository is an official PyTorch implementation of (["Small Scale Data-Free Knowledge Distillation", SSD-KD for short](https://github.com/OSVAI/SSD-KD)), accepted to CVPR 2024. 

Data-free knowledge distillation (D-KD) is able to utilize the knowledge learned by a large teacher network to augment the training of a smaller student network without accessing the original training data, avoiding privacy, security, and proprietary risks in real applications. In this line of research, existing methods typically follow an inversion-anddistillation paradigm in which a generative adversarial network on-the-ﬂy trained with the guidance of the pre-trained teacher network is used to synthesize a large-scale sample set for knowledge distillation. In this paper, we reexamine this common data-free knowledge distillation paradigm, showing that there is considerable room to improve the overall training effciency through a lens of “small-scale inverted data for knowledge distillation”. In light of three empirical observations indicating the importance of how to balance class distributions in terms of synthetic sample diversity and diffculty during both data inversion and distillation processes, we propose Small Scale Data-free Knowledge Distillation (SSD-KD, the below figure shows a schematic comparison of our SSD-KD with exisiting D-KD methods). In formulation, SSD-KD introduces a modulating function to balance synthetic samples and a priority sampling function to select proper samples, facilitated by a dynamic replay buffer and a reinforcement learning strategy. As a result, SSD-KD can perform distillation training conditioned on an extremely small scale of synthetic samples (e.g., 10× less than the original training data scale), making the overall training effciency one or two orders of magnitude faster than many mainstream methods while retaining superior or competitive model performance, as demonstrated on popular image classifcation and semantic segmentation benchmarks.

![teaser](./framework_ssd-kd.png)

## Code will be coming soon. Stay tuned.
