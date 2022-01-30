# Multi-ClothNet: Automatic Cloth Size Measurement using Multitask Learning Based CNNs
In this study, we design a set of equipment to capture images of clothes of any style and any color, and propose an automatic size measurement approach which consists of two steps (i.e., Landmarks localization and physical dimensions measurement).For landmarks detection, we propose a novel multitask learning based network which exploits the additional knowledge of cloth segmentation to optimize the learning for landmarks detection. We also propose a dataset **CDMD - Cloth Dimension Measurement Dataset ** that allows to convert measurements in pixels into measurements in physical length.
## Pipeline

As shown in the image, in this pipeline, we utilized multitask semi-supervised network, that uses adversarial autoencoder to encode the useful features. These features are further utilized for landmark detection (main task) and segmentation (auxiliary task).

![Complete pipeline](https://github.com/Azkarehman/Multi-ClothNet/blob/main/images/complete_mod.png|width=1000px)

## Dataset
The dataset consists of five different categories of cloth images. These categories include skirt, top, cardigan, pants, dress. This dataset is unique because it allows to convert measurements in pixels into measurements in physical length. Some example images are shown below:
![Dataset](https://github.com/Azkarehman/Multi-ClothNet/blob/main/images/Picture2.png =250x250)

## Results:
Sample results for lower body cloths:

|                     | Skirt      | Pants      |
|---------------------|------------|------------|
| Measurement         | % Accuracy | % Accuracy |
|                     |            |            |
| Length              | 97.4       | 99.8       |
| Waist Circumference | 98         | 96.6       |
| Trouser Hem         | -          | 95.4       |
| Hem Circumference   | 90         | -          |
| Hips Circumference  | 98.2       | 96.5       |
| Mean Accuracy       | 95.9       | 97         |

## Project Development phase:

 - Data collection 
 - Data cleaning 
 - Data preprocessing  
 - Research and development phase 
 - Finalizing the solution     
 - Integrating the solution
## Technical Details
**Language:** Python
**Deep learning Framework:** Keras
**Image Processing libraries:** Opencv, Scikit learn

