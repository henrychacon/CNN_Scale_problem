# CNN scale invariance problem

In this project, the parallel GPU process included in the Tourch package is used to train a traditional LeNet-5 architecture proposed by LeCun in 1989:

![image1](https://github.com/henrychacon/CNN_invariance_transformation/blob/master/images/convolution_cnnlecun.png)

The model was trained using the MNIST data set and tested using four different scales: 1/2, 1/3, 2 and 3. Some examples are presented below:

![image2](https://github.com/henrychacon/CNN_Scale_problem/blob/master/images/Scaled%20examples.png)

Since the convolution operation is not scaled invariance, the feature detection in the first convolution layer of the model is not able to get the same sequence of the non-scale image. The difference in the first layer between the original image and the scaled image for the number seven is presented in the following image:

![image3](https://github.com/henrychacon/CNN_Scale_problem/blob/master/images/ErrorLayer.png)

The global per target label using all the possible scaling transformation is illustrated in the figure. Notice that the label one is the less sensitive to scaling transformation, due to the shape does not have any curve. Finally, the sampling distribution of the error for each scaling combination is presented, Bootstrap was used for this task.

![image4](https://github.com/henrychacon/CNN_Scale_problem/blob/master/images/GeneralErrorpercategory.png)
![image5](https://github.com/henrychacon/CNN_Scale_problem/blob/master/images/distribution.png)
