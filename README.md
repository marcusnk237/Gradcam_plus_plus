# Gradcam_plus_plus
one of the first implementation of Grad-CAM ++ (https://doi.org/10.1109/WACV.2018.00097)  for time series / 1d signal.   The module  gives a visual explainations of the decisions made by Deep Learning model (Especially for classification problems). GRAD-CAM++ helps to understand how the model works and assert the model results.
Two outputs modes are available :
- The output can be an image, with the signal as the foreground and the heatmap as the background
![Alt text](https://github.com/marcusnk237/Gradcam_plus_plus/blob/main/results_gradcam/gradcam_plus_plus_2d.png)

- The output can be the signal with each important segment draw with a color which represent the importance for the classification/prediction
![Alt text](https://github.com/marcusnk237/Gradcam_plus_plus/blob/main/results_gradcam/gradcam_plus_plus_1d.png)

Sources :
Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks :https://doi.org/10.1109/WACV.2018.00097
