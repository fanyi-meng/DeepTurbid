![image](https://github.com/user-attachments/assets/526f6e14-d590-4393-a51d-7e322f755b2a)

Using fiducial markers for visual localization provides a robust solution for long-duration underwater positioning. However, image degradation caused by water turbidity often leads to the failure of traditional, hand-crafted detection methods. To address this challenge, we introduce **DeepTurbid**, a system for underwater marker detection and pose estimation. Building on existing ArUco marker systems, DeepTurbid defines the mapping of marker control points in challenging underwater environments and employs a high-resolution neural network for keypoint prediction and marker ID decoding. Moreover, by leveraging the underwater imaging model and the optical properties of underwater scenes, we propose an underwater marker image generation scheme and an adaptive heatmap labeling. This approach generates a diverse marker image dataset, spanning multiple water types and degradation levels for network training. We evaluate DeepTurbid in challenging real-world turbid underwater environments, and experimental results demonstrate that our method significantly outperforms existing approaches in terms of marker detection robustness and pose estimation accuracy.

**Note:** The code, dataset, and full experimental details will be released **only after** the paper is accepted. Until then, this repository may include preliminary content or placeholders.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Current Status](#current-status)
- [Network Architecture](#network-architecture)
- [Dataset Showcase](#dataset-showcase)
- [Experimental Results](#experimental-results)
- [Installation](#installation)
- [Usage](#usage)
- [Citation](#citation)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

---

## Overview

DeepTurbid is designed to provide robust underwater marker detection and pose estimation, specifically addressing the challenges posed by water turbidity. The system leverages a high-resolution neural network that:
- **Predicts keypoints** for marker detection.
- **Decodes marker IDs** from degraded images.
- **Utilizes an underwater imaging model** to generate diverse training data with adaptive heatmap labeling.

This comprehensive approach ensures that DeepTurbid remains effective even under severely degraded underwater conditions.

---

## Features

- **Robust Detection in Turbid Environments:** Overcomes limitations of traditional hand-crafted methods using deep learning.
- **Accurate Pose Estimation:** Provides reliable marker pose estimation in challenging underwater scenarios.
- **Adaptive Data Generation:** Simulates various water types and degradation levels via an underwater marker image generation scheme.
- **High-Resolution Neural Network:** Utilizes a state-of-the-art architecture for precise keypoint prediction and marker ID decoding.
- **Diverse Dataset:** Covers multiple water conditions for robust network training.

---

## Current Status

- **Paper Status:** Submitted (Under Review)
- **Open-Source Policy:** The code, dataset, and complete experimental details will be released **only after** the paper is accepted.
- **Development:** Until the paper is accepted, this repository may be updated with preliminary work or placeholders.

---

## Network Architecture

This section provides an overview of the network structure used in DeepTurbid.

- **Network Diagram:**  
![Net2](https://github.com/user-attachments/assets/ca1710e9-55d5-4dd4-a4cd-73afc411b267)

*More detailed network configuration and parameters will be available upon open-source release.*

---

## Dataset Showcase

This section demonstrates the dataset used to train and evaluate DeepTurbid.

- **Dataset Overview:**  
  DeepTurbid leverages both synthetic and real-world datasets that cover a range of water types and degradation levels.
![Dataset_generated_](https://github.com/user-attachments/assets/2c93b566-ecbc-4b01-8782-a2521552f6bb)

- **Dataset Samples:**  
![image](https://github.com/user-attachments/assets/e1848c8e-02eb-483e-8ac4-5dc2e70ece56)
![image](https://github.com/user-attachments/assets/0ae780bd-f6af-404d-9bef-3861234496f8)
![image](https://github.com/user-attachments/assets/babdb891-14de-494d-95c2-979011372b1b)
![image](https://github.com/user-attachments/assets/1a016364-60ce-485f-9846-de4a766e16c6)

- **Dataset Structure:**  

  ```plaintext
  /dataset
  ├── images/         # Underwater marker images
  ├── annotations/    # Annotations including keypoints and marker IDs
  └── README.md       # Dataset description and usage instructions

## Visual Results


https://github.com/user-attachments/assets/fd252b6e-59f0-4e0b-8916-2c618069cad9


![marker_4_q](https://github.com/user-attachments/assets/5bdec864-b35b-472e-9f8c-292c6aa94c1a)![marker_999_manual](https://github.com/user-attachments/assets/0c57c094-6437-4b3e-a646-144be738f3cb)
![marker_123_roi_expanded_ids](https://github.com/user-attachments/assets/8b560849-c358-48af-a25f-bf42016dbe5f)
![marker_123_roi_expanded](https://github.com/user-attachments/assets/e0e3d3b7-5d75-4264-a269-51713b36ac2d)
![marker_123_q](https://github.com/user-attachments/assets/c30c4c57-d496-420a-9329-93cabd80129c)
![marker_123_bb](https://github.com/user-attachments/assets/49501796-ba93-43aa-bff2-b817e14f264c)
![marker_4_q_ids](https://github.com/user-attachments/assets/24e25f6c-ff47-4882-aa65-27073a84754c)








