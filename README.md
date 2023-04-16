# BSRGAN Degradation Model


The degradation model used in BSRGAN. It is meant to provide a better method of obtaining the low-quality (LQ) images from their high-quality (HQ) counterparts. These LQ images will then be subsequently used as the input of an Image Super-Resolution model such as SRGAN, ESRGAN, SwinIR, etc.

This is meant to provide a better starting point then the commonly used bicubic downsampling (usually MATLAB's "imresize" function). The transformations provided by this degradation model create LQ images which are closer to the images we find in the wild than what we would get by simply applying a bicubic downsampling.

The exact degradation pipeline is discussed in the official paper titled ["Designing a Practical Degradation Model for Deep Blind
Image Super-Resolution"](https://arxiv.org/abs/2103.14006) and the code was taken from the official [GitHub repository](https://github.com/cszn/BSRGAN). 

Nothing new is implemented here as far as the transformations go, this repository is just a convinient place to have the transformations used in BSRGAN.


<img width="1152" alt="image" src="https://user-images.githubusercontent.com/72063186/232308379-15026542-175e-441b-9099-0cb4ad64b7df.png">

NB: Forked from the [official implementation](https://github.com/cszn/BSRGAN) and only kept the degradation code.
