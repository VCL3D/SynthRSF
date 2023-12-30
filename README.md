# SynthRSF Dataset

## Overview
SynthRSF is a synthetic, photorealistic dataset designed for training and evaluating single-image denoising algorithms under adverse weather conditions like rain, snow, and haze. It includes 26,893 noisy images, each paired with a corresponding ground truth image.

## Features
- **Weather Types:** Rain, snow, uniform and non-uniform fog.
- **Image Pairs:** Each noisy frame has a corresponding ground truth image.
- **Depth Maps and Annotations:** Accompanied by 16-bit depth maps and pixel-accurate annotations for various objects.
- **Use Cases:** Ideal for object detection, semantic segmentation, and depth estimation in noisy or denoised images.

## Access
The dataset is available on the Git repository: [SynthRSF Repository](https://github.com/VCL3D/SynthRSF).

---

# SynthRSF-MM Dataset

## Overview
SynthRSF-MM is an expansion of the SynthRSF dataset, including additional modalities for a comprehensive analysis in computer vision tasks. It contains 13,800 noisy images from 14 scenes with ground truth on additional modalities.

## Features
- **Multi-Modal Data:** Includes depth map, semantic segmentation, and bounding box pixel coordinates for 39 classes.
- **Unique Scenes:** Manually populated with various 3D objects, including persons, vehicles, animals, etc.
- **Annotations:** Equipped with YOLO-compatible bounding box .json files and pixel-accurate segmentation per object instance.
- **Applications:** Suitable for tasks such as object detection, image segmentation, depth estimation, and more.

## Access
For more details and access to the dataset, visit the Git repository: [SynthRSF-MM Repository](https://github.com/VCL3D/SynthRSF).

---

# Additional Information

Both datasets were created using the Unreal 5.2 game engine, ensuring high photorealism and accurate simulation of weather conditions. They serve as valuable resources for developing and testing image restoration models under challenging weather conditions.

---

Note: Always ensure compliance with the usage guidelines and terms provided in the respective repositories.
