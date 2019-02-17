**A honey bee (Apis)**

![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/Bee-apis.jpg/337px-Bee-apis.jpg)

**A Bumble Bee (Bombus)**

![](https://cdn6.picsart.com/6469671680.jpeg?c256x256)

Can a machine identify a bee as a honey bee or a bumble bee? These bees have different behaviors and appearances, but given the variety of backgrounds, positions, and image resolutions, it can be a challenge for machines to tell them apart.

### Use Case

Being able to identify bee species from images is a task that ultimately would allow researchers to more quickly and effectively collect field data. Pollinating bees have critical roles in both ecology and agriculture, and diseases like colony collapse disorder threaten these species. Identifying different species of bees in the wild means that we can better understand the prevalence and growth of these important insects.

### Steps (Part 3)

1. Explore the data format
2. Create function to access all images in folder
3. Normalize all the RGB (color) values of each image
4. Train-test-split the data for a validation set (evaluation set) and training set
5. Building a Sequential convolutional neural network.
6. Adding varying layers to the model
   - Maxpooling (reduce dimensionality)
   - Two Dropout layers (prevent overfitting)
   - Flatten data into one dimension
7. Compile the model
   - SGD Optimizer (good at generalizing, but time consuming)
   - Loss Function set to binary cross entropy
   - metrics = accuracy
   - Epochs = 200 (10 used as a test)
8. Fit and evaluate the data
   - Examine the loss and accuracy on the test and validation set
   - Use the History Object to examine the history of scores as the ephocs go up
   - Generate predictions and probabilities
   
### Next Steps

Deploy the model using flask to make it accesable, and perform tests on new data. 
