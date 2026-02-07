# 102316104_UCS654_Assignment4_GAN
## Dataset: 
Consider NO2 concentration as the feature ( x ).

Dataset link: https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data
## Transformation
z = x + a_r*sin(b_r *x)

where 

a_r = 0.5 (r mod 7)

b_r = 0.3 (r mod 5 + 1)

## Transformation Parameter
ar=1.0,br=1.5
## GAN Architecture
A simple fully connected GAN is employed, where the generator takes 1-D Gaussian noise as input and learns a nonlinear mapping to approximate the target data distribution. The discriminator is a multi-layer perceptron trained to classify real samples and generator-produced samples, enabling adversarial learning.
## GAN Training Loss Log

| Epoch | Discriminator Loss (D) | Generator Loss (G) |
|-------|------------------------|--------------------|
| 0     | 1.404                  | 0.652              |
| 200   | 1.255                  | 0.595              |
| 400   | 1.389                  | 0.869              |
| 600   | 1.367                  | 0.676              |
| 800   | 1.363                  | 0.723              |
| 1000  | 1.383                  | 0.681              |
| 1200  | 1.386                  | 0.689              |
| 1400  | 1.381                  | 0.746              |
| 1600  | 1.428                  | 0.793              |
| 1800  | 1.377                  | 0.729              |
| 2000  | 1.379                  | 0.654              |
| 2200  | 1.381                  | 0.686              |
| 2400  | 1.398                  | 0.729              |
| 2600  | 1.395                  | 0.679              |
| 2800  | 1.370                  | 0.710              |
| 3000  | 1.417                  | 0.721              |
| 3200  | 1.384                  | 0.726              |
| 3400  | 1.380                  | 0.677              |
| 3600  | 1.385                  | 0.729              |
| 3800  | 1.381                  | 0.673              |
| 4000  | 1.397                  | 0.646              |
| 4200  | 1.390                  | 0.715              |
| 4400  | 1.375                  | 0.702              |
| 4600  | 1.380                  | 0.671              |
| 4800  | 1.386                  | 0.684              |
##
