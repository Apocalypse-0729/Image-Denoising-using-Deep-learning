

![Image](https://imgs.search.brave.com/54RuFOSCS1ZIouO0AmqAs8eUeYw-XTDrg9kECUpvD4s/rs:fit:500:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5saWNkbi5jb20v/ZG1zL2ltYWdlL0M1/MTFCQVFFc0ZZODVD/YnRsRmcvY29tcGFu/eS1iYWNrZ3JvdW5k/XzEwMDAwLzAvMTU4/NTM5NzEwODcyOC92/bGdpaXRyX2NvdmVy/P2U9MjE0NzQ4MzY0/NyZ2PWJldGEmdD04/VUFVZmtmcVJJcXRD/RkFzOHFzTlNfSEJu/UkU3dUJaYXNyM01M/UHFGM2VF.jpeg)
# Image-Denoising-using-Deep-learning

## INRODUCTION
### What is Noise in an image?
The images that are captured in the real world come with noises. These noises can appear due to many reasons such as electric signal instabilities, malfunctioning of camera sensors, poor lighting conditions, errors in data transmission over long distances, etc. So, there is a need to remove these noises from images when it comes to low-level vision tasks and image processing. The process of removing such noises from images is known as Image Denoising. 
Image noise is a random variation of brightness or color information in the images captured. It is degradation in image signal caused by external sources. Mathematically, noise in an image can be represented by,
A(x,y) = B(x,y) + H(x,y)
Where,
A(x,y) = function of noisy image
B(x,y) = function of original image
H(x,y) = function of noise

#### Performance Metrics
**Peak Signal to Noise Ratio (PSNR)** - The term peak signal-to-noise ratio (PSNR) is an expression for the ratio between the maximum possible value (power) of a signal and the power of distorting noise that affects the quality of its representation.  Because many signals have a very wide dynamic range, (ratio between the largest and smallest possible values of a changeable quantity) the PSNR is usually expressed in terms of the logarithmic decibel scale. The higher the PSNR, the better the quality of the compressed image.

![Alt text](https://i.ibb.co/PTV3qds/PSNR-Formula.png)
                         
### METHODOLOGIES USED
#### Results from AutoEncoder

### Building of Model-
![Alt text](https://i.ibb.co/z5m3bc3/Auto-Encoder-Model.png)
 
### Model Fitting-
![Alt text](https://i.ibb.co/xz5bC7P/Auto-Encoder-Model-Fitting.png)
 
### Noising Factor-
![Alt text](https://i.ibb.co/zsLCv6t/Auto-Encoder-Noise-Factor.png)

### Predicted data-
![Alt text](https://i.ibb.co/FqYv3nL/Auto-Encoder-Predicted-Data.png)

### Noised Testing data-
![Alt text](https://i.ibb.co/Q9k5YvN/Auto-Encoder-Test-Data.png)

### Average PSNR value-
![Alt text](https://i.ibb.co/6b83rmd/Auto-Encoder-PSNR-AVERAGE.png)
 
#### Zero DCE (Zero-Reference Deep Curve Estimation) –
This method trains a lightweight deep network, DCE-Net, to estimate pixel-wise and high-order curves for dynamic range adjustment of a given image. The curve estimation is specially designed, considering pixel value range, monotonicity, and differentiability. It does not require any paired or unpaired data during training. This is achieved through a set of carefully formulated non-reference loss functions, which implicitly measure the enhancement quality and drive the learning of the network. This method is efficient as image enhancement can be achieved by an intuitive and simple nonlinear curve mapping. A Deep Curve Estimation Network (DCE-Net) is devised to estimate a set of best-fitting Light-Enhancement curves (LE-curves) given an input image. The framework then maps all pixels of the input’s RGB channels by applying the curves iteratively for obtaining the final enhanced image.
The input to the DCE-Net is a low-light image while the outputs are a set of pixel-wise curve parameter maps for corresponding higher-order curves. It is a plain CNN of seven convolutional layers with symmetrical concatenation. Each layer consists of 32 convolutional kernels of size 3×3 and stride 1 followed by the ReLU activation function.
 
![Alt text](https://i.ibb.co/QXXpXH7/DCE-Explain2.png)

![Alt text](https://i.ibb.co/6tyqvV7/DCE-Explain.png)

### Building of Model-
![Alt text](https://i.ibb.co/RypqcB4/DCE-Model.png)

### Testing data-
![Alt text](https://i.ibb.co/JpGXsJV/DCE-Dataset.png)

### Training and Testing of data-
![Alt text](https://i.ibb.co/zSFRNVz/DCE-Training-and-Testing.png)

### Average PSNR value-
![Alt text](https://i.ibb.co/0fSjMrR/DCE-PSNR.png)
 


### REFERENCES
1.	https://medium.com/analytics-vidhya/noise-removal-in-images-using-deep-learning-models-3972544372d2
2.	https://www.youtube.com/watch?v=ggJhpgXK6E0
3.	https://github.com/sunilbelde/Imagedenoising-dncnn-ridnet-keras/tree/main/code
4.	https://medium.com/analytics-vidhya/image-denoising-using-deep-learning-dc2b19a3fd54





