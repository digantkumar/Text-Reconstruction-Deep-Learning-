
1. Tasks for Basic Autoencoder Assignment
As you may see after training this model, the reconstructed images are quite blurry. A number of things could be done to move forward from this point, e.g. adding more layers, or using a convolutional neural network architecture as the basis of the autoencoder, or use a different kind of autoencoder.

generate results for 3 different Dense architectures and summarise the impact of architecture on performance
define 2 CNN architectures (similar to as described) and compare their performance to that of the Dense models
Since our inputs are images, it makes sense to use convolutional neural networks (CNNs) as encoders and decoders. In practical settings, autoencoders applied to images are always convolutional autoencoders -- they simply perform much better.

implement a CNN model, where the encoder will consist of a stack of Conv2D and MaxPooling2D layers (max pooling being used for spatial down-sampling), while the decoder will consist in a stack of Conv2D and UpSampling2D layers. To improve the quality of the reconstructed image, we use more filters per layer

2. Tasks for Denoising Autoencoder Assignment

models [5 marks]:
Dense, multi-layer model 
CNN basic model [given]
CNN complex model [5 marks].
results and discussion [5 marks]: present the results in a clear fashion and explain why the results were as obtained. Good experimental design and statistical significance testing will be rewarded.

3. Text Reconstruction Application

You will now use the approach just described to reconstruct corrupted text. We will use a small dataset with grey-scale images of size $420 \times 540$. The steps required are as follows:

Apply this autoencoder approach (as just described) to the text data provided as noted below.
The data has two sets of images, train (https://github.com/gmprovan/CS6421-Assignment1/blob/master/train.zip) and test (https://github.com/gmprovan/CS6421-Assignment1/blob/master/test.zip). These images contain various styles of text, to which synthetic noise has been added to simulate real-world, messy artifacts. The training set includes the test without the noise (train_cleaned: https://github.com/gmprovan/CS6421-Assignment1/blob/master/train_cleaned.zip).
You must create an algorithm to clean the images in the test set, and report the error as RMSE (root-mean-square error).
Scoring: 40 marks total

models [25 marks]:
Dense, multi-layer model [5 marks];
CNN basic model [5 marks];
CNN complex models (at least 2) [15 marks].
results and discussion [15 marks]: present the results in a clear fashion and explain why the results were as obtained. Good experimental design and statistical significance testing will be rewarded.
