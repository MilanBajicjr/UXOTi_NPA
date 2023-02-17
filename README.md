# UXOTi_NPA 11 class UXO thermal images dataset
UXOTi_NPA dataset authored by Milan jr. Bajić, Božidar Potočnik

Evaluation dataset UXOTi_NPA–an abbreviation that stands for UneXploded Ordnance Thermal images provided by Norwegian People's Aid–for this research was constructed as follows. The raw data was provided by the humanitarian organization Norwegian People’s Aid which collected videos about unexploded ordnances during a project in Bosnia and Herzegovina in 2019. Thermal imaging sensor was mounted on the UAV that surveyed the area at a height of 3 meters. A very small Ground Sampling Distance (GSD) was achieved with such a configuration. These videos were acquired by the thermal imager Zenmuse XT with a dimension of 720x480 pixels at 30 Hz frame rate. Pixel pitch was 17 μm, sensitivity (NEdT) <50mK at focal length f/1.0, and a field of view was 69°x56°. Videos were stored in mp4 format. Image sequences were grabbed from the full videos by using VirtualDub software. These clips were about 25 seconds long and show the UAV's flight over the targets. We annotated videos semi-automatically by using Computer Vision Annotation Tool (CVAT). Positions of objects’ annotations were manually corrected after every 5 to 6 frames. The evaluation dataset consists of 808 thermal images of dimensions of 720x480 pixels extracted from the above-described video clips, whenever at least one target (UXO) was present in the image. The number of objects per image varied between one to three. 
Files can be accessed here https://figshare.com/articles/dataset/UXOTi_NPA_11_class_dataset/21688661 and here https://figshare.com/articles/dataset/UXOTi_NPA_1_class_dataset/21688673

If you find UXOTi_NPA dataset useful in your research, please cite:

    @Article{rs15040967,
    AUTHOR = {Bajić, Milan and Potočnik, Božidar},
    TITLE = {UAV Thermal Imaging for Unexploded Ordnance Detection by Using Deep Learning},
    JOURNAL = {Remote Sensing},
    VOLUME = {15},
    YEAR = {2023},
    NUMBER = {4},
    ARTICLE-NUMBER = {967},
    URL = {https://www.mdpi.com/2072-4292/15/4/967},
    ISSN = {2072-4292},
    DOI = {10.3390/rs15040967}
    
ABSTRACT

A few promising solutions for thermal imaging Unexploded Ordnance (UXO) detection were proposed after the start of the military conflict in Ukraine in 2014. At the same time, most of the landmine clearance protocols and practices are based on old, 20th-century technologies. More than 60 countries worldwide are still affected by explosive remnants of war, and new areas are contaminated almost every day. To date, no automated solutions exist for surface UXO detection by using thermal imaging. One of the reasons is also that there are no publicly available data. This research bridges both gaps by introducing an automated UXO detection method, and by publishing thermal imaging data. During a project in Bosnia and Herzegovina in 2019, an organisation, Norwegian People&rsquo;s Aid, collected data about unexploded ordnances and made them available for this research. Thermal images with a size of 720 &times; 480 pixels were collected by using an Unmanned Aerial Vehicle at a height of 3 m, thus achieving a very small Ground Sampling Distance (GSD). One of the goals of our research was also to verify if the explosive war remnants&rsquo; detection accuracy could be improved further by using Convolutional Neural Networks (CNN). We have experimented with various existing modern CNN architectures for object identification, whereat the YOLOv5 model was selected as the most promising for retraining. An eleven-class object detection problem was solved primarily in this study. Our data were annotated semi-manually. Five versions of the YOLOv5 model, fine-tuned with a grid-search, were trained end-to-end on randomly selected 640 training and 80 validation images from our dataset. The trained models were verified on the remaining 88 images from our dataset. Objects from each of the eleven classes were identified with more than 90% probability, whereat the Mean Average Precision (mAP) at a 0.5 threshold was 99.5%, and the mAP at thresholds from 0.5 to 0.95 was 87.0% up to 90.5%, depending on the model&rsquo;s complexity. Our results are comparable to the state-of-the-art, whereat these object detection methods have been tested on other similar small datasets with thermal images. Our study is one of the few in the field of Automated UXO detection by using thermal images, and the first that solves the problem of identifying more than one class of objects. On the other hand, publicly available thermal images with a relatively small GSD will enable and stimulate the development of new detection algorithms, where our method and results can serve as a baseline. Only really accurate automatic UXO detection solutions will help to solve one of the least explored worldwide life-threatening problems.



