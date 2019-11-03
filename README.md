# CV-digit-recognition

DIGIT RECOGNITION USING OPENCV

These are the steps that are needed to detect handwritten digits -

1.Create a database of handwritten digits.
2.For each handwritten digit in the database, extract HOG features and train a Linear SVM.
3.Use the classifier trained in step 2 to predict digits.


MNIST DATABASE
Here, we use the MNIST database as the database.The MNIST database is a set of 70000 samples of handwritten digits where each sample consists of a grayscale image of size 28×28. There are a total of 70,000 samples. We will use sklearn.datasets package to download the MNIST database from mldata.org. 

TRAINING THE CLASSIFIER
We will implement the following steps –

1.Calculate the HOG features for each sample in the database.
2.Train a multi-class linear SVM with the HOG features of each sample along with the corresponding label.
3.Save the classifier in a file

LOADING THE CLASSIFIER
Then we load the classifier and use it in the code.
