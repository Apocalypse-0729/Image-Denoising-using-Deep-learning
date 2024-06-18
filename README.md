
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
Peak Signal to Noise Ratio (PSNR) - The term peak signal-to-noise ratio (PSNR) is an expression for the ratio between the maximum possible value (power) of a signal and the power of distorting noise that affects the quality of its representation.  Because many signals have a very wide dynamic range, (ratio between the largest and smallest possible values of a changeable quantity) the PSNR is usually expressed in terms of the logarithmic decibel scale. The higher the PSNR, the better the quality of the compressed image.
                         
### METHODOLOGIES USED
#### Results from AutoEncoder
![Alt text](blob/master/Images/AutoEncoder_Model.png)
### Building of Model-
 
### Model Fitting-
 
### Noising Factor-
 
### Predicted data-
 
### Noised Testing data-
 
### Average PSNR value-
 
#### Zero DCE (Zero-Reference Deep Curve Estimation) –
This method trains a lightweight deep network, DCE-Net, to estimate pixel-wise and high-order curves for dynamic range adjustment of a given image. The curve estimation is specially designed, considering pixel value range, monotonicity, and differentiability. It does not require any paired or unpaired data during training. This is achieved through a set of carefully formulated non-reference loss functions, which implicitly measure the enhancement quality and drive the learning of the network. This method is efficient as image enhancement can be achieved by an intuitive and simple nonlinear curve mapping. A Deep Curve Estimation Network (DCE-Net) is devised to estimate a set of best-fitting Light-Enhancement curves (LE-curves) given an input image. The framework then maps all pixels of the input’s RGB channels by applying the curves iteratively for obtaining the final enhanced image.
The input to the DCE-Net is a low-light image while the outputs are a set of pixel-wise curve parameter maps for corresponding higher-order curves. It is a plain CNN of seven convolutional layers with symmetrical concatenation. Each layer consists of 32 convolutional kernels of size 3×3 and stride 1 followed by the ReLU activation function.
 



### REFERENCES
1.	https://medium.com/analytics-vidhya/noise-removal-in-images-using-deep-learning-models-3972544372d2
2.	https://www.youtube.com/watch?v=ggJhpgXK6E0
3.	https://github.com/sunilbelde/Imagedenoising-dncnn-ridnet-keras/tree/main/code
4.	https://medium.com/analytics-vidhya/image-denoising-using-deep-learning-dc2b19a3fd54





