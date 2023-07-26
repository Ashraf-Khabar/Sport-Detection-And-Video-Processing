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

* We used `Pytorch` for model creation, and tensor creations : 

  <a href="https://nodejs.org/en/"> <img src="https://cdn.icon-icons.com/icons2/2699/PNG/512/pytorch_logo_icon_169823.png" alt="php" height="100"></a>
* We used `sklearn` for metrics and performance : 

  <a href="https://nodejs.org/en/"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png" alt="php" height="90"></a>
* We used `numpy` for ndarray manupilation befor transforme it to `torch tensors` : 

  <a href="https://nodejs.org/en/"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png" alt="php" height="100"></a>

## Additional Details Of The CNN Model

* `SGD` (Stochastic Gradient Descent) Optimizer:

The SGD optimizer is a widely used optimization algorithm for training machine learning models. The update step for each parameter is computed using the following formula:

$\theta_{new} = \theta_{old}-(\alpha \times \nabla\mathcal{L(x, \mathscr{C}) - (\mathrm{momentum } \times \mathrm{previousUpdate} ) - (\mathrm{weightDecay} * \theta_{old})})$

with : 

* $\theta_{new}$ : is the updated value of the parameter.
- $\theta_{old}$ : is the current value of the parameter.
* $\alpha$ : is the learning rate hyperparameter, controlling the step size during updates.

* $\nabla\mathcal{L(x, \mathscr{C})}$ : is the gradient of the loss function with respect to the parameter.
* $\mathrm{momentum }$ : is the momentum hyperparameter, which smooths the update process and helps to accelerate convergence in certain cases.
* $\mathrm{previousUpdate}$ : is the accumulated previous update for the parameter.
* $\mathrm{weightDecay}$ :  is the weight decay hyperparameter, which applies L2 regularization to the parameter to prevent overfitting.

in `Python` and `Pytorch` :

```py
optimizer = optim.SGD(model.fc.parameters(), lr=0.001, momentum=0.9, weight_decay=1e-4)
```
* `CrossEntropyLoss`:

CrossEntropyLoss is a common loss function used for classification tasks. The formula for the CrossEntropyLoss is as follows:

$\mathcal{L}(x, \mathscr{C}) = \frac{-\log(e^{x_c})}{\sum_{i=1}^{n}e^{x_i}}$

with : 

* $x$ is the output (logits) from the last layer of the neural network for a particular input.

* $\mathscr{C}$ is the true class label of the input.

* $x_{c}$ is the input for the class $\mathscr{C}$.