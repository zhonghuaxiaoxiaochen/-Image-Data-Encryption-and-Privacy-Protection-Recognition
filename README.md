# -Image-Data-Encryption-and-Privacy-Protection-Recognition
This project is the code part of the paper "An Encrypted Image Recognition Scheme Based on Edge Detection and Steganography".

1. Data preparation

  CIFAR10
  The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.
  The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each     class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them,   The training batches contain exactly 5000 images from each class.
  CIFAR100
  This dataset is just like the CIFAR-10, except it has 100 classes containing 600 images each. There are 500 training images and 100 testing images per class. 
  The 100 classes in the CIFAR-100 are grouped into 20 superclasses.
  Each image comes with a "fine" label (the class to which it belongs) and a "coarse" label (the superclass to which it belongs).
  The download from：http://www.cs.toronto.edu/~kriz/cifar.html

2. Data preprocessing
  The experimental data must be converted into Visible data in jpg or other formats (saved into two copies for experiment), which is convenient for later data processing.
  
3. Experiment
  ① Take one of them The jpg image data adopts the improved Canny edge detection algorithm for edge detection to obtain the edge detection result image.
  ② Another. jpg image data is encrypted with the improved Lorenz chaotic encryption algorithm to obtain the encrypted image.
  ③ The edge detection results are steganographic into the encrypted image using frequency domain steganography.
  ④ Stealth the extracted image for ResNet18 network recognition test.
