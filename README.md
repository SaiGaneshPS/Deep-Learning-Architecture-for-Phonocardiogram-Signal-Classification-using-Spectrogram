# Deep-Learning-Architecture-for-Phonocardiogram-Signal-Classification-using-Spectrogram
Using a deep learning architecture to classify PCG signals that are read from .wav files.

Dataset : https://www.kaggle.com/lilpegasus/spectogram

The image dataset after conversion consists of *3240* images in total.

 - Abnormal = 665 Images
 - Normal = 2575 Images

From the above numbers, it is evident that the data is skewed towards one class (Normal),
so the required data augmentation is done to increase the number of images in Abnormal class.

After data augmentation, the dataset split is :

 - Abnormal = 2660 Images
 - Normal = 2575 Images

============================================================================================================================
Steps to completely classify PCG signals :
1. Read the input .wav files and convert them to images using spectograms.
2. Using the spectograms as images, build a CNN architecture to classify these images.
3. Train the CNN model and classify the test data.

============================================================================================================================
** CNN Architecture 

Starting from the input layer :
![image](https://user-images.githubusercontent.com/60283852/152285565-9b287e44-6d2c-453a-9852-6b8837b221c0.png)

To the final dense layer :
![image](https://user-images.githubusercontent.com/60283852/152285585-43aa2cc3-94aa-4c01-90a7-c597f8cf8e63.png)

============================================================================================================================
The final accuracy obtained is 92%.

The results for the same dataset in different circumstances :

![image](https://user-images.githubusercontent.com/60283852/152285440-eee33895-e737-4b78-a164-4edb07c217b3.png)
