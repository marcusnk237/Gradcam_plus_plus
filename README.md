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

Clone the repo
   ```
   sh git clone https://github.com/marcusnk237/Gradcam_plus_plus.git
   ```
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage
```

compute_cam_1d_output (model, data , layer_name , N)
Arguments:
> - model : The model trained
> - data : The data sample
> - layer_name : The last layer of the feature extraction part of the model. Usually, it is the last layer before the Flattening operation.
> - N : data length
```
![Alt text](https://github.com/marcusnk237/dataset_gradcam_plus_plus/blob/main/results/gradcam_plus_plus_1d.png)


<!-- CONTACT -->
## Contact
* [![LinkedIn][linkedin-shield]][linkedin-url]

* Project Link: [https://github.com/marcusnk237/Gradcam_plus_plus](https://github.com/marcusnk237/Gradcam_plus_plus)
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
[Matplotlib]:https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black
[Matplotlib-url]:https://matplotlib.org/
[NumPy]: https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white
[Numpy-url]:https://numpy.org/
[Python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=yellow
[Python-url]: https://www.python.org/
[Tensorflow]: https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white 
[Tensorflow-url]:  https://www.tensorflow.org/


