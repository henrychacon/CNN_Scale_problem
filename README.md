# CNN scale invariance problem

In this project, the parallel GPU process included in the Tourch package is used to train a traditional LeNet-5 architecture proposed by LeCun in 1989:

![image1](https://github.com/henrychacon/CNN_invariance_transformation/blob/master/images/convolution_cnnlecun.png)

The model was trained using the MNIST data set and tested using four different scales: 1/2, 1/3, 2 and 3. Some examples are presented below:

![image2](https://github.com/henrychacon/CNN_Scale_problem/blob/master/images/Scaled%20examples.png)

Since the convolution operation is not scale invariance, the feature detection in the first convolution layer of the model is not able to get the same sequence of the non scale image. The difference in the first layer between the original image and the scaled image for the number seven is presented in the following image:

