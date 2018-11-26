# HyperGAN: A Generative Model for Neural Networks
![arch](imgs/arch.png)

HyperGAN generates fully trained neural networks simply by sampling from noise. 
No large dataset of fully trained examples needed. 
We use repeated MLE estimates to bring the generators closer to generating samples from the true distribution
In the end, we have fully trained neural networks that can be instantly generated. 
Large ensembles are trivial to create and expand. 

Generating a huge ensemble (100-1000 or more networks) allows us to fully approximate the learned distribution of neural networks. 
Allowing us to make advances in anomaly detection and uncertainty estimation. 

# Train a HyperGAN

## 1-D Regression

```
python3 hypertoy_regression.py --pretrain_e True
```

## MNIST
``` 
python3 hypermnist.py --pretrain_e True 
```

## MNIST 5000
```
python3 hypermnist5000.py --pretrain_e True
```

## CIFAR-10
```
python3 hypercifar.py --pretrain_e True
```

## CIFAR-10 5000
```
python3 hypercifar5000.py --pretrain_e True
```
