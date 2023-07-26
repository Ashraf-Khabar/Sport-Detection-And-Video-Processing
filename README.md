# <center style="color:#d589">Sport Detection And Video Processing</center>

* This project aims to create a deep learning model for extracting items from a sports video and accurately detecting the type of sport featured in the video .
* In this `Model` we will use a dataset of images classed by names, for example :

    ```js
    {
        'Basketball': [
            image_1, 
            image_2, 
            image_3,
            ...
        ],
        'Football'  : [...],
        'Hockey' : [...],
        ...
    }
    ```
* We exctract the images in order to train the `CNN` with `PyTorch` .
* We will save the model and use it in video processing and in order to detect the sport playing in the video . 

## Python Libraries 

* We used `Pytorch` for model creation, and tensor creations : 

  <a href="https://nodejs.org/en/"> <img src="https://cdn.icon-icons.com/icons2/2699/PNG/512/pytorch_logo_icon_169823.png" alt="php" height="100"></a>
* We used `sklearn` for metrics and performance : 

  <a href="https://nodejs.org/en/"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png" alt="php" height="90"></a>
* We used `numpy` for ndarray manupilation befor transforme it to `torch tensors` : 

  <a href="https://nodejs.org/en/"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png" alt="php" height="100"></a>

## Additional Details Of The CNN Model

