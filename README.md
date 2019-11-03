# CV-digit-recognition


Basic steps followed are:-
1)Create a database of handwritten digits.
2)For each handwritten digit in the database, extract HOG features and train a Linear SVM.
3)Use the classifier trained in step 2 to predict digits.

MNIST DATABASE


The MNIST database is a set of 70000 samples of handwritten digits where each sample consists of a grayscale image of size 28×28. There are a total of 70,000 samples. It is downloaded from  http://yann.lecun.com/exdb/mnist/.The training files are extracted and then given as input.

CLASSIFIER

We will use the sklearn.externals.joblib package to save the classifier in a file so that we can use the classifier again without performing training each time. We use skimage.feature.hog class to calculate the HOG features and sklearn.svm.LinearSVCclass to perform prediction after training the classifier. We store our HOG features and labels in numpy arrays. 

PREDICTION


We predict the digits by loading the classifier created in our code.
