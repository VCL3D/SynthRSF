# SynthRSF Dataset

## Overview
- SynthRSF (Synthetic with Rain, Snow, uniform and non-uniform Fog) dataset is introduced for **training and evaluating adverse weather image denoising models** as well as use in **object detection, semantic segmentation, and depth estimation** models.
- SynthRSF addresses a gap in synthetic datasets for adverse weather conditions, contributing significantly more photorealistic data compared to common 2D layered noise datasets, as well as additional modalities. 
- Applications include autonomous driving, surveillance, robotics, computer-assisted search-and-rescue.

## Contents
- **SynthRSF:** 
  - 26,893 photorealistic image pairs (noisy and ground truth).
  - 14 3D scenes set in various environmental (rural/urban), contextual (indoor/outdoor) and lighting conditions (day/night).
  - Created using Unreal 5.2 engine.


- **SynthRSF-MM expansion:**
  - 13,800 additional pairs are accompanied by: 
  - 16-bit depth maps.
  - Pixel-accurate object annotations for 41 object classes.

## SynthRSF Examples
<table>
  <tr>
    <td colspan="2">
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene3_rain_noisy_14122.jpeg" width="350px" />
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene16_rain_noisy_07084.jpeg" width="350px" /><br>
      <em>Rain</em>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_snow_2_noisy_00180.jpeg" width="350px" />
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene16_snow_noisy_11562.jpeg" width="350px" /><br>
      <em>Snow</em>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene14_fog_homogenous_noisy_00210.jpeg" width="350px" />
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene6_fog_homogenous_noisy_07080.jpeg" width="350px" /><br>
      <em>Uniform Fog</em>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene1_fog_heterogenous_noisy_00422.jpeg" width="350px" />
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_fog_heterogenous_noisy_00021.jpeg" width="350px" /><br>
      <em>Non-Uniform Fog</em>
    </td>
  </tr>
</table>




# SynthRSF-MM Dataset

## Overview
SynthRSF-MM is an expansion of the SynthRSF dataset, including additional modalities for a comprehensive analysis in computer vision tasks. It contains 13,800 noisy images from 14 scenes with ground truth on additional modalities.

## SynthRSF-MM Example


<table>
  <tr>
    <td>
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_GT_068.jpg" width="300px" /><br>
      <em>Ground truth</em>
    </td>
    <td>
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_Depth_068.jpg" width="300px" /><br>
      <em>Depth map</em>
    </td>
    <td>
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/stencil.png" width="300px" /><br>
      <em>Object annotations</em>
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_Fog_068.jpg" width="300px" /><br>
      <em>Fog</em>
    </td>
    <td>
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_Rain_068.jpg" width="300px" /><br>
      <em>Rain</em>
    </td>
    <td>
      <img src="https://github.com/VCL3D/SynthRSF/blob/main/figures/Scene4_Snow_068.jpg" width="300px" /><br>
      <em>Snow</em>
    </td>
  </tr>
</table>




*A sample scene from SynthRSF-MM, showing the ground truth (clear) scene, depth map, semantic segmentation stencil mask, and three noisy variants with different weather conditions. For each Ground truth image, there is one depth map, five pixel-level annotations and 8 noisy images per phenomenon.*




---
  
# SynthRSF Source 3D Scenes

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
# SynthRSF-MM Source 3D Scenes

| No | Description        | Ground Truth | Depth | Snow | Rain | Fog (NU) |
|----|--------------------|--------------|-------|------|------|----------|
| 1  | CitySample day     | 226          | 226   | 1808 | 1808 | 1808     |
| 2  | CitySample night   | 158          | 158   | 1264 | 1264 | 1264     |
| 3  | Archviz Interior   | 32           | 32    | -    | -    | 256      |
| 4  | Factory            | 32           | 32    | -    | -    | 256      |
| 5  | OfficeVol1         | 102          | 102   | -    | -    | 816      |
| 6  | Bedroom Vol 1      | 22           | 22    | -    | -    | 176      |
| 7  | Kitchenette        | 22           | 22    | -    | -    | 176      |
| 8  | MegascansAA        | 20           | 20    | -    | -    | 160      |
| 9  | MegascansSnow      | 20           | 20    | 160  | 160  | 160      |
| 10 | Desert             | 17           | 17    | 136  | 136  | 136      |
| 11 | MeerkatDemo        | 21           | 21    | 168  | 168  | 168      |
| 12 | ICVFXProdTest      | 21           | 21    | 168  | 168  | 168      |
| 13 | AngryMesh W1       | 21           | 21    | 168  | 168  | 168      |
| 14 | AngryMesh W2       | 21           | 21    | 168  | 168  | 168      |
|    | **Total**          | **825**      | **825**| **4040**|**4040**| **5720** |
---

# Access
The dataset is available on Google Drive: https://drive.google.com/drive/folders/1UiXTYSIWbX2w62E-WDjxMyDGWvWDF0oX?usp=drive_link

It is free to use for research purposes, provided the original paper is cited:

Kanlis, A.; Vanian, V.; Karvarsamis, S.; Gkika, I.; Konstantoudakis, K. and Zarpalas, D. (2024). SynthRSF: A Novel Photorealistic Synthetic Dataset for Adverse Weather Condition Denoising.  In Proceedings of the 19th International Joint Conference on Computer Vision, Imaging and Computer Graphics Theory and Applications - Volume 3: VISAPP, ISBN 978-989-758-679-8, ISSN 2184-4321, pages 567-574.  DOI: 10.5220/0012397700003660  


---

 
