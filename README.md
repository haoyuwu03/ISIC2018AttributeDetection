# ISIC2018AttributeDetection
Duke +Datascience 2022 Spring Research Program
Skin Lesion Analysis Toward Melanoma Detection 2018: A Challenge Hosted by the International Skin Imaging Collaboration (ISIC)
Detecting symptoms of Malignant Melanoma (skin cancer) from dermoscopic images from the ISIC 2018 Challenge Dataset:
https://challenge.isic-archive.com/landing/2018/

About the dataset:
- Largest public collection of quality controlled dermoscopic images of skin lesions with 13,000 images
- Acquired from a variety of devices from leading international clinical centers
- Incoming images are screened for privacy and quality including vetting of clinical metadata by melanoma experts
- A subset are annotated for dermoscopic features by skin cancer experts
- Dermoscopy improves diagnostic accuracy by eliminating surface reflection of skin to visualize deeper levels
- Patient care could be improved with inexpensive dermatoscope attachments for smartphones alongside automated diagnosis 
- 2594 Training Images, 100 Validation, 100 Test
- Number of images for each lesion:
  - Globules: 603 train 19 val
  - Milia Like Cyst: 682 train 6 val
  - Pigment Network: 1523 train 73 val
  - Negative Pigment Network: 190 train 9 val
  - Streaks: 100 train 6 val
- Size of input: 256 x 256 x 3
- Color scale: RGB

Model Architecture Used:


Example Results of UNET (64 starting filters, 0.2 dropout, 10^-4 learning rate, threshold: 1.2 times positive pixel ratio in masks):

![Pigment Network](https://github.com/haoyuwu03/ISIC2018AttributeDetection/blob/main/UNET_Globule_Detection_Results.png)
