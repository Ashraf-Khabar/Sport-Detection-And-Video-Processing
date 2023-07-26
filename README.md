# <center style="color:#d589">Sport Detection And Video Processing</center>

* This porject aimes to make a deep learning model in order to extract items from a sport video in order to detect which sport is in the video . 
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


1. Model creation and tensor manipulations were performed using `PyTorch`:
   ![PyTorch Logo](https://cdn.icon-icons.com/icons2/2699/PNG/512/pytorch_logo_icon_169823.png)

2. Metrics and performance evaluation were conducted with the help of `scikit-learn`:
   ![scikit-learn Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png)

3. To handle ndarray manipulation before transforming it into `torch tensors`, we relied on `NumPy`:
   ![NumPy Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png)