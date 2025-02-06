# DeepTurbid: Underwater Marker Detection and Pose Estimation

Using fiducial markers for visual localization provides a robust solution for long-duration underwater positioning. However, image degradation caused by water turbidity often leads to the failure of traditional, hand-crafted detection methods. To address this challenge, we introduce **DeepTurbid**, a system for underwater marker detection and pose estimation. Building on existing ArUco marker systems, DeepTurbid defines the mapping of marker control points in challenging underwater environments and employs a high-resolution neural network for keypoint prediction and marker ID decoding. Moreover, by leveraging the underwater imaging model and the optical properties of underwater scenes, we propose an underwater marker image generation scheme and an adaptive heatmap labeling. This approach generates a diverse marker image dataset, spanning multiple water types and degradation levels for network training. We evaluate DeepTurbid in challenging real-world turbid underwater environments, and experimental results demonstrate that our method significantly outperforms existing approaches in terms of marker detection robustness and pose estimation accuracy.

The code and dataset are publicly available at [DeepTurbid GitHub Repository](https://github.com/fanyi-meng/DeepTurbid).

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Evaluation](#evaluation)
- [Results](#results)
- [Citation](#citation)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

---

## Overview

DeepTurbid is designed to provide robust underwater marker detection and pose estimation, specifically addressing the challenges posed by water turbidity. The system leverages a high-resolution neural network that:
- Predicts keypoints for marker detection.
- Decodes marker IDs from degraded images.
- Utilizes an underwater imaging model to generate diverse training data with adaptive heatmap labeling.

This approach ensures that DeepTurbid remains effective even in severely degraded underwater conditions.

---

## Features

- **Robust Detection in Turbid Environments:** Overcomes limitations of traditional hand-crafted methods through deep learning.
- **Accurate Pose Estimation:** Provides reliable marker pose estimation in challenging underwater conditions.
- **Adaptive Data Generation:** Employs an underwater marker image generation scheme to simulate various water types and degradation levels.
- **High-Resolution Neural Network:** Utilizes state-of-the-art architecture for precise keypoint prediction and marker ID decoding.
- **Diverse Dataset:** Generates a comprehensive dataset covering multiple water conditions for robust network training.

---

## Installation

### Prerequisites

- Python 3.7 or later
- [PyTorch](https://pytorch.org/) (or your preferred deep learning framework)
- OpenCV
- NumPy
- Additional dependencies (refer to `requirements.txt`)

### Setup Instructions

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/fanyi-meng/DeepTurbid.git
   cd DeepTurbid
