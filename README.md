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

* We used Pytorch