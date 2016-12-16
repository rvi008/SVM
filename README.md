# TP SVM

## Question 1
We load the Iris Dataset and train a simple Linear Kernel SVM.
The fiting score is 66%.
We get a cross validated score of 72% +/-16% accuracy.

## Question 2
We now train a polynomial kernel SVM and get a fiting score of 72% (better) but the  cross validated score is 72% +/- 16%. No improvement

## Question 3 
See Notebook

## Question 4
The classification error 1 or 0 has 2 shelves, so we can't minimise this constant by chunk and discountinuous function.
We use the Hinge function which is majorating the error function (see plot in notebook).
It is a convex function so we can minimise it with a gradient descent.

## Question 5
We can see in the plot that as C increases, the prediction error decreases until it's stable.
The coefficient tunes the number of classification errors we accept when larger we accept less errors.*

## Question 6
As expected when we add columns of noise the performances decreases but the rate is not so strong 

## Question 7
The features are standardized because the SVM algorithm lays on distances calculations. So we need to reduce the importance
of the big values.

## Question 8
The plot clearly shows that the performances are significantly lower than those
of the linear kernel SVM.
