# SignLanguageRecognizer
__Contributers:__ [Aybuke Yalciner](https://github.com/AybukeYALCINER "GitHub"), [Furkan Caglayan](https://github.com/furkancaglayan "GitHub"), [Enes Furkan Cigdem](https://github.com/Enescigdem)



## 1.License
This work is licensed under [MIT license](https://github.com/furkancaglayan/SignLanguageRecognizer/blob/master/LICENSE).

## 2.Dataset
We created our own dataset and used 24 different gestures/letter signs. Images are taken from 2 different signers and there are **1560** train samples, **360** validation and **360** test data. We preferred to use pretrained VGG model as classifier and achieved **99%** accuracy. But you are free yo use the dataset however you like.

## 3.Prerequisites

### OpenCV
### PyTorch and TorchVision



In this study, we collect our own dataset and used 24 different gestures. Images are taken from 2 people and there are 1560 train data,
360 validation and 360 test data. We prefer to use pretrained VGG model as classifier. After we train the model, we come up with about 
%99 accuracy on test data.

<p align="center">
  <img src="right.png" width="550" title="screen" align="center">  
</p>
  
The above picture shows the right part of the system. We display the segmented hand in res window, some information in detailed window and 
some controller in information window to control the upper and lower RGB values according to light in th environment. To change the 
lower and upper RGB values, the OF...ON should be switched to 1. 

Additionally, while system is running, 
<br> 
* If "b" is pressed from keyboard, the binary segmented form of the frame is shown in the res window.
* If "c" is pressed from keyboard, the segmented form of the frame is shown in the res window(it is also default).     
* If "h" is pressed from keyboard, the the extracted features using hog of the frame is shown in the res window.
* If "s" is pressed from keyboard, the segmented form of the frame which is converted to grayscale is saved.

Medium blog:
https://medium.com/@aybukeyalcinerr/realtime-recognition-of-american-sign-language-alphabet-8ece006d424e?postPublishedType=repub

