# Gradcam_plus_plus
<a name="readme-top"></a>
<br />
<div align="center">
  <h1 align="center">Grad-CAM ++ for time series classification</h1>

</div>
<!-- TABLE OF CONTENTS -->
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-code">About</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>


<!-- ABOUT THE PROJECT -->
## About The Project


One of the main challenges in artificial intelligence for the researchers is to understands how model predictions works.
Many contributions has been made, especially GRAD-CAM++.
Grad-CAM++ give a visual representation of the keys features responsible of the classification, and give human-level understanding of the model prediction. 
Despite its advantages, GRAD-CAM ++ is not initially design for time series

The program give a GRAD-CAM ++ visualisation for time series

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

[![Python][Python]][Python-url]
[![Tensorflow][Tensorflow]][Tensorflow-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
[![Tensorflow][Tensorflow]][Tensorflow-url]
[![Opencv][Opencv]][Opencv-url]
[![Matplotlib][Matplotlib]][Matplotlib]
[![Numpy][Numpy]][Numpy-url]

### Installation

1. Clone the repo
   ```
   sh git clone https://github.com/marcusnk237/dataset_gradcam_plus_plus.git
   ```
2. Install the library
   ```
   python3 setup.py install
   ```
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage
### Local visual explanation
```
from dataset_gradcam_plus_plus  import local_features_importances
local_features_importances(model,data,time,layer_name,label)
Arguments:
> - model : The model trained
> - data : The data sample
> - time : The time range (The user can create a linspace vector and use it as the time range).
> - layer_name : The last layer of the feature extraction part of the model. Usually, it is the last layer before the Flattening operation.
> - label : The label output list
```
![Alt text](https://github.com/marcusnk237/dataset_gradcam_plus_plus/blob/main/results/gradcam_plus_plus_1d.png)

### Dataset level feature relevance
```
from dataset_gradcam_plus_plus import dataset_features_importances

dataset_features_importances(model,datas,layer_name,feature_names,flag=True)

Arguments:
> - model : The model trained
> - datas : the dataset. Due of Hardware limitations, the max size of datas is 5000 samples.
> - layer_name : The last layer of the feature extraction part of the model. Usually, it is the last layer before the Flattening operation.
> - feature_names : The feature list
> - flag : True, return the global feature importance plot; False, return the feature importance frequency and the corresponding features
```
![Alt text](https://github.com/marcusnk237/dataset_gradcam_plus_plus/blob/main/results/dataset_level_feature_importance.jpg)
<!-- LICENSE -->
## License

Distributed under the GNU License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact
* [![LinkedIn][linkedin-shield]][linkedin-url]

* Project Link: [https://github.com/marcusnk237/dataset_gradcam_plus_plus](https://github.com/marcusnk237/dataset_gradcam_plus_plus)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

The authors of the original article about GRAD-CAM++
* [Aditya Chattopadhay; Anirban Sarkar; Prantik Howlader; Vineeth N Balasubramanian : Grad-CAM++: Generalized Gradient-Based Visual Explanations for Deep Convolutional Networks](https://doi.org/10.1109/WACV.2018.00097)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/marcusnk237/dataset_gradcam_plus_plus/blob/main/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/marc-junior-nkengue/
[product-screenshot]: images/screenshot.png

[Opencv]:https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white
[Opencv-url]:https://pypi.org/project/opencv-python/
[Pandas]:https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white
[Pandas-url]:https://pandas.pydata.org/
[Matplotlib]:https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black
[Matplotlib-url]:https://matplotlib.org/
[NumPy]: https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white
[Numpy-url]:https://numpy.org/
[Python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=yellow
[Python-url]: https://www.python.org/
[Tensorflow]: https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white 
[Tensorflow-url]:  https://www.tensorflow.org/


