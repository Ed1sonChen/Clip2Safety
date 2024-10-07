# Clip2Safety: Vision Language Model for Interpretable and Fine-grained Detection of Safety Compliance in Diverse Workplaces
This is the official implementation of paper "Vision Language Model for Interpretable and Fine-grained Detection of Safety Compliance in Diverse Workplaces".

> Zhiling Chen*, Hanning Chen, Mohsen Imani, Ruimin Chen, Farhad Imani.
>
> Paper Link: https://arxiv.org/pdf/2408.07146

## Overview

The variability in safety gear across industries, such as construction and manufacturing, makes it difficult for models to consistently detect the appropriate equipment. Complex work environments further complicate detection and verification of PPE compliance with industry-specific standards. Current models often fail to generalize across different settings, leading to inaccurate results. Additionally, aligning visual data with textual descriptions of PPE remains a challenge, especially when verifying fine-grained attributes like material type or durability. 

<img src="./Figures/introduction.png" alt="Clip2Safety" style="zoom:50%;" />


## Framework

This paper addresses the challenge of workplace safety compliance across various industries by introducing Clip2Safety, a framework leveraging vision-language models (VLMs) for fine-grained PPE detection. Traditional safety inspections rely on manual labor or sensor-based systems, which struggle with generalization across diverse work environments. Additionally, these systems face challenges in detecting nuanced variations in safety gear attributes required for different industries.

Clip2Safety resolves these challenges through a two-stage reasoning framework. First, an object detection model isolates individuals and their safety gear in images. Then, a VLM compares these cropped images with text descriptions to ensure not only the presence of required safety gear but also its compliance with specific attributes necessary for safety. This method eliminates the need for extensive fine-tuning while maintaining adaptability across different industries, leveraging zero-shot learning to generalize to new scenarios. The system has been tested across six distinct environments, demonstrating its effectiveness in enhancing safety compliance detection.

<img src="./Figures/model.png" alt="Clip2Safety" style="zoom:50%;" />

## Citation
```
@article{chen2024vision,
  title={Vision Language Model for Interpretable and Fine-grained Detection of Safety Compliance in Diverse Workplaces},
  author={Chen, Zhiling and Chen, Hanning and Imani, Mohsen and Chen, Ruimin and Imani, Farhad},
  journal={arXiv preprint arXiv:2408.07146},
  year={2024}
}
```

