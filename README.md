# Traffic Signs Dataset with extreme weather conditions
> **Supported Figures for scientific paper:**  
> *EXTENDED TRAFFIC SIGNS DATASET WITH EFFECTS OF EXTREME WEATHER CONDITIONS*  
> Valentyn N. Sichkar, Dmitry I. Mouromtsev  
  
<img src="figures/Fig.%201.%20Distribution.png" width=50%>  
Fig. Distribution of the images among classes in the original dataset  

# 

<img src="figures/Fig.%202.%20Example%20of%20the%20augmentation.png" width=50%>
Fig. Example of the augmentation stages via affine transformations. 1st row: original images, 2nd row: rotation around centre point, 3rd row: elastic distortion, 4th row: horizontal shear, 5th row: all three previous techniques together  

#

<img src="figures/Fig.%203.%20Histograms%20of%20the%20pixel%20values%20density.png" width=50%>
Fig. Histograms of the pixel values density for the rain and snow masks in the gray colour space. 1st row from left to right: minimum rain and snow. 2nd row from left to right: medium rain and snow. 3rd row from left to right: maximum rain and snow  

#

<img src="figures/Fig.%2019.%20Localized%20and%20classified%20traffic%20signs%20in%20heavy%20snow.png" width=50%>
Fig. Example of the image from localization dataset with applied mask of the weather conditions  

#

<img src="figures/Fig.%2010.%20Architecture%20of%20deep%20CNN.png" width=50%>
Fig. Architecture of deep CNN model for classification

#

<img src="figures/Fig.%2011.%20Comparison%20of%20the%20validation%20accuracies%20.png" width=50%>
Fig. Comparison of the validation accuracies obtained during training of the classification model. 1st row from left to right: accuracies of the baseline model trained on original dataset and model trained on v1 dataset. 2nd row from left to right: accuracies of the model trained on v2 dataset and model trained on v3 dataset. 3rd row from left to right: accuracies of the model trained on v4 dataset and model trained on v5 dataset

#

<img src="figures/Fig.%2012.%20Comparison%20of%20the%20validation%20losses.png" width=50%>
Fig. 12. Comparison of the validation losses obtained during training of the classification model. 1st row from left to right: losses of the baseline model trained on original dataset and model trained on v1 dataset. 2nd row from left to right: losses of the model trained on v2 dataset and model trained on v3 dataset. 3rd row from left to right: losses of the model trained on v4 dataset and model trained on v5 dataset

#

<img src="figures/Fig.%2013.%20mAp0.5%20obtained%20from%20baseline%20YOLO.png" width=50%>
Fig. mAp@0.5 obtained from baseline YOLO v4 model trained on GTSDB and its 43 classes

#

<img src="figures/Fig.%2015.%20mAp0.5%20obtained%20from%20YOLO.png" width=50%>
Fig. mAp@0.5 obtained from YOLO v4 model with 4 super-classes and 5 versions of the GTSDB dataset

#

<img src="figures/Fig.%2016-1.%20Localized%20traffic%20signs%20.png" width=50%>
<img src="figures/Fig.%2016-2.%20Localized%20traffic%20signs.png" width=50%>
Fig. Localized traffic signs in a good weather condition and with extreme rain

#

<img src="figures/Fig.%2017.%20Localized%20and%20classified%20traffic%20signs%20in%20heavy%20rain.png" width=50%>
Fig. Localized and classified traffic signs in heavy rain weather conditions. On the right side: localized fragments that are sent to the classification part of the proposed recognition model

#

<img src="figures/Fig.%2018.%20Localized%20traffic%20signs%20in%20heavy%20snow.png" width=50%>
Fig. Localized traffic signs in heavy snow weather conditions


#

<img src="figures/Fig.%2019.%20Localized%20and%20classified%20traffic%20signs%20in%20heavy%20snow.png" width=50%>
Fig. Localized and classified traffic signs in heavy snow weather conditions. On the right side: localized fragments that are sent to the classification part of the proposed recognition model

#

`Table. Hyperparameters to train classification model `  

Hyperparameter |	Version Original |	v1, v2, v3, v4, v5
------------- | -------------  | -------------
Epochs |	50 |	50
Batch size |	50 |	50
Iterations |	726 |	1813
Weights initializer |	Glorot uniform |	Glorot uniform

# 

`Table. Hyperparameters to train baseline YOLO v4 localization model`

Hyperparameter |	Value
------------- | -------------
Network size |	608 × 608
Batch size | 64
Subdivisions	| 32
Learning rate	| 0.001
Learning rate decay	| 0.0005
Anchors, scale 1 (small object)	| (12, 16), (19, 36), (40, 28)
Anchors, scale 2 (medium object)	| (36, 75), (76, 55), (72, 146)
Anchors, scale 3 (large object) | (142, 110), (192, 243), (459, 401)
Saturation	| 1.5
Exposure	| 1.5
Hue	| 0.1

#

`Table. Grouping 43 classes into 4 super-classes`
Super-class	| Related class indexes | Related	group description
------------- | -------------  | -------------
1 |	0, 1, 2, 3, 4, 5, 7, 8, 9, 10, 15, 16	| Circular traffic signs with white background and red border line
2	| 11, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31	| Triangular traffic signs with white background and red border line
3	| 33, 34, 35, 36, 37, 38, 39, 40	| Circular traffic signs with blue background
4	| 6, 12, 13, 14, 17, 32, 41, 42	| All other types of traffic signs

