# RSNA-Fracture-Detection
## Goal of the Competition
Over 1.5 million spine fractures occur annually in the United States alone resulting in over 17,730 spinal cord injuries annually. The most common site of spine fracture is the cervical spine. There has been a rise in the incidence of spinal fractures in the elderly and in this population, fractures can be more difficult to detect on imaging due to superimposed degenerative disease and osteoporosis. Imaging diagnosis of adult spine fractures is now almost exclusively performed with computed tomography (CT) instead of radiographs (x-rays). Quickly detecting and determining the location of any vertebral fractures is essential to prevent neurologic deterioration and paralysis after trauma.

## Context
RSNA has teamed with the American Society of Neuroradiology (ASNR) and the American Society of Spine Radiology (ASSR) to conduct an AI challenge competition exploring whether artificial intelligence can be used to aid in the detection and localization of cervical spine fractures.

To create the ground truth dataset, the challenge planning task force collected imaging data sourced from twelve sites on six continents, including approximately 3,000 CT studies. Spine radiology specialists from the ASNR and ASSR provided expert image level annotations these studies to indicate the presence, vertebral level and location of any cervical spine fractures.

In this challenge competition, you will try to develop machine learning models that match the radiologists' performance in detecting and localizing fractures to the seven vertebrae that comprise the cervical spine. Winners will be recognized at an event during the RSNA 2022 annual meeting.

For more information on the challenge, contact RSNA Informatics staff at informatics@rsna.org.

A full set of acknowledgments can be found on this page.

## About Dataset
#### This dataset contains metadata extracted from train image dicom files relevant to the RSNA 2022 Cervical Spine Fracture Detection competition.
1. meta-train - original metadata extracted (ignore this file)
2. meta-train-clean - cleaned version of meta-train (easier to use)
3. meta-segmentations - meta-data for images with segmentations (including correct labels C1-C7 extracted from unique values in segmentations)
4. meta-train-with-vertebrae - meta-data for all train images (with 88% accurate RF predictions of which vertebrae is in each image)
5. train-segmented - meta-data for all train images (with 95% accurate EffNetV2 predictions of which vertebrae is in each image from this notebook)

#### The notebooks used to create these files are below:
1. RSNA Fracture Detection - in-depth EDA
2. Extracting Vertebrae C1, …, C7
