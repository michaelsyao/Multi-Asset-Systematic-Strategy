# ReinforementLearning.DNN.RNN
```
This section forcuses on ReinforementLearning and DNN 
```
## A. Use Dense Neutral Network for FX price discovery
#### Use couple techniques to increase Out of sample prediction power
> 1. Normalization: Gaussian normalization
> 2. Drop out: Not use all hidden units during the training stage.
> 3. Regularization: Large weights in the neural network get penalized in the calculation of the loss (function).
> 4. Bagging: Avoid overfitting
> 5. Optimizers: 

| Optimizer   | Description               |
| ----------- | ------------------------- |
| sgd         | LearningRateSchedule      |
| rmsprop     | root mean square propagation        |
| adagrad     | Adaptive Gradient Optimizer        |
| adadelta    | A more robust extension of Adagrad that seeks to reduce its aggressive, monotonically decreasing learning rate based on a fixed moving window of gradient updates, instead of accumulating all past gradients.        |
| adam    | adaptive moment estimation        |
| adamax    | extension to Adam         |
| nadam    | Nesterov-accelerated Adaptive Moment Estimation        |

## Result

|       | Baseline| Normalization|Drop out| Reg| Bagging| Optimizer|
| ----- | -------- |------------|--------|----------|----------|------|
| Train      | 59.3% | 92.1% | 77.5% | 89.4% | 76.1% | Adam
| Test   | 61.3% |67.7%|64.5%|67.2% |66.6%| 64.7%|

1. [DenseNeutralNetwork for FX](HierarchicalRiskParity.ipynb)

## B. Use Recurrent Neutral Network for FX price discovery
> Project 1: Use Dense Neutral Network along with Normalization and Bagging technique to increase performance 
1. [Dense Neutral Network](Proj1_DNN_FX.ipynb)

