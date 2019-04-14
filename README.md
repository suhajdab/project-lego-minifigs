# Project Lego minifigs
### Experiment for generating Lego Minifigures using a Deep Convolutional Generative Adversarial Network

This experiment was inspired while completing the [Face Generation](https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-face-generation) project of the Udacity [Deep Learning](https://eu.udacity.com/course/deep-learning-nanodegree--nd101) nanodegree.

The training data for this experiment was scraped from [bricklink](https://www.bricklink.com/catalogTree.asp?itemType=M&itemBrand=1000), and thus will not be published along with the code. I manually removed photos of unusual figures, those of low quality and or containing multiple figures. Then, as most photos did not have sufficient room to be cropped into a square, I scaled and padded the photos to 256x256 pixels. I ended up with a dataset of 6100+ photos. 

The good: ![good](https://img.bricklink.com/ItemImage/MT/0/s011.t1.png)
The bad: ![bad](https://img.bricklink.com/ItemImage/MT/0/cc4064.t1.png)
The ugly: ![ugly](https://img.bricklink.com/ItemImage/MT/0/njo188.t1.png)

While I've managed to generate some images that begin to look like minifigs, I'm not satisfied with the results.
The images are still very blurry and the network exploded around 150 epochs, and never recovered.

**Suggestions on how to overcome these issues would be much appreciated!**
