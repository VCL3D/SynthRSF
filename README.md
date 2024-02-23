# SynthRSF Dataset

## Overview
SynthRSF is a synthetic, photorealistic dataset designed for training and evaluating single-image denoising algorithms under adverse weather conditions like rain, snow, and haze. It includes 26,893 noisy images, each paired with a corresponding ground truth image.

## Features
- **Weather Types:** Rain, snow, uniform and non-uniform fog.
- **Image Pairs:** Each noisy frame has a corresponding ground truth image.
- **Use Cases:** Training weather denoising models.


| No | Description        | Snow | Rain  | Fog (U) | Fog (NU) |
|----|--------------------|------|-------|---------|----------|
| 1  | CitySample day     | 3862 | 10758 | 522     | 430      |
| 2  | CitySample night   | 2695 | 2744  | -       | -        |
| 3  | Hillside Sample    | 485  | 412   | 254     | 308      |
| 4  | AngryMesh W1       | 279  | 287   | 180     | 211      |
| 5  | AngryMesh W2       | 400  | 377   | 171     | 170      |
| 6  | ICVFXProdTest      | -    | -     | 8       | 14       |
| 7  | Realistic Rend.    | -    | -     | 75      | 75       |
| 8  | Archviz Interior   | -    | -     | -       | 30       |
| 9  | Factory            | -    | -     | 13      | 16       |
| 10 | Office Vol. 1      | -    | -     | 45      | 38       |
| 11 | Bedroom Vol. 1     | -    | -     | 246     | 203      |
| 12 | Kitchenette        | -    | -     | 3       | 15       |
| 13 | Megascans A. A.    | -    | -     | 19      | 42       |
| 14 | MeerkatDemo        | 250  | 250   | 51      | 55       |
|    | **Total**          | **7971** | **14828** | **1487**   | **1607**   |
---

# SynthRSF-MM Dataset

## Overview
SynthRSF-MM is an expansion of the SynthRSF dataset, including additional modalities for a comprehensive analysis in computer vision tasks. It contains 13,800 noisy images from 14 scenes with ground truth on additional modalities.

## Features
- **Multi-Modal Data:** Includes depth map, semantic segmentation, and bounding box pixel coordinates for 39 classes.
- **Unique Scenes:** Manually populated with various 3D objects, including persons, vehicles, animals, etc.
- **Annotations:** Equipped with YOLO-compatible bounding box .json files and pixel-accurate segmentation per object instance.
- **Applications:** Suitable for tasks such as object detection, image segmentation, depth estimation, and more.
- **Depth Maps and Annotations:** Accompanied by 16-bit depth maps and pixel-accurate annotations for various objects.
- **Use Cases:** Ideal for object detection, semantic segmentation, and depth estimation in noisy or denoised images.
 
---

# Access
The dataset is available on Google Drive: https://drive.google.com/drive/folders/1UiXTYSIWbX2w62E-WDjxMyDGWvWDF0oX?usp=drive_link

---


# Additional Information

Both datasets were created using the Unreal 5.2 game engine, ensuring high photorealism and accurate simulation of weather conditions. They serve as valuable resources for developing and testing image restoration models under challenging weather conditions.

---

Note: Always ensure compliance with the usage guidelines and terms provided in the respective repositories.
