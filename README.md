# Real-time image-based parking occupancy detection and automatic parking slot deliniation using deep learning: A tutorial
This is the MATLAB tutorial of our upcoming Book Chapter (will update the details soon). We provide a MATLAB [Live Script](https://github.com/DebadityaRMIT/Parking/blob/master/FinalCode.mlx) (.mlx file) that is pre-compiled MATLAB file containing all the results, and the corresponding [PDF document](https://github.com/DebadityaRMIT/Parking/blob/master/FinalCode.pdf) for convinience. 

There are two tutorials that are presented to obtain results on a sample dataset (and the trained weight files) that we publically share at [this link](https://rmit.figshare.com/ndownloader/files/24753887). The first tutorial involves fine-tuning a pre-trained deep neural network for vehicle detection in a sequence of CCTV camera images to determine the occupancy of the parking spaces. Also, we provide insights on the training hyper-parameters, training and testing times, accuracies and visualise some wrong classifications. For a CPU-friendly version using a CNN + SVM framework, please follow [our previous work here](https://github.com/debaditya-unimelb/real-time-car-parking-occupancy). 

In the second tutorial, we combined the detections in multiple frames and performed spatio-temporal analysis of the parking slots to automatically delineate the parking slots. We used a robust density-based clustering algorithm to find the centre of the parking slots, and then weighted the bounding boxes according to the detection scores (confidence). We further post-processed the delineations to improve the detection accuracy.

The tutorial is intended to run on MATLAB 2020a, although the code can run in MATLAB versions higher than 2018a. Additional toolboxes might be required to run the experiments that include computer vision toolbox, statistics and machine learning toolbox, deep learning toolbox, signal processing toolbox and automated driving toolbox. For running the live script smoothly, please ensure to increase the java heap memory of MATLAB, as demonstrated at the start of the live script.

[![ProjectImage](https://github.com/DebadityaRMIT/Parking/blob/master/ProjectThumbnail.png)](https://github.com/DebadityaRMIT/Parking/blob/master/FinalCode.pdf)

Please cite our work if you use any part of the code:
```
Acharya, D., Yan, W., Khoshelham, K., 2018. Real-time image-based parking occupancy detection using deep learning.
In: Proceedings of the 5th Annual Conference of Research@Locate, Adelaide, Australia, CEUR Workshop Proceedings, 
vol. 2087, pp. 33???40. 

```
```
@inproceedings{Deb:acharya2018real,
	title={Real-time image-based parking occupancy detection using deep learning},
	author={Acharya, Debaditya and Yan, Weilin and Khoshelham, Kourosh},
	booktitle={Proceedings of the 5th Annual Conference of Research@Locate}, 
	year={2018},
	month = {April},
	pages={33-40},
	volume={2087}
}
```
