# SC5002_LabAssignment2_Group10
This is the Github repository of group 10 (Nguyen Tuan Minh, Ribbe Linnea, and Sim Yee Hang Bryan) for lab assignment 2 of module SC5002. 

## Downloading the Project
To use this program, download/clone the entire project to your local computer.

* If you are a git user, you can clone the most current version of the repository:

<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;git clone https://github.com/NguyenTuanMi/SC5002_LabAssignment2_Group10.git</p>

* Or, if you prefer, you can use the "Download Zip" button available through the main repository page.  Downloading the project as a .ZIP file will keep the size of the download manageable.

## Requirement
To use this project, please first download Jupyter Notebook or open this in web browser

## Flow of the program
### Data Processing (Bryan)

* Through plotting graphs of numerical and categorical datatypes, we learn that the dataset is highly biased and the distribution of prices and areas are not normal. However, the distribution are right-skewed, we suspect that through log transformation on prices and areas, normality could be obtained.

### Model training and Evaluation (Minh Nguyen)

* We use Linear Regression and Ridge Regression models. For ridge regression, we evaluate 100 values of alpha in a range from 10^-3 to 10^2. The best alpha is around 35, giving us roughly 71% R^2 score in testing dataset and 65% R^2 score in training dataset.

### Analysis (Linnea)

* We realize that we might experiencing underfitting: our models are too simple to capture the data patterns (the accuracies are low, the MSE errors are high).

### Improvement (Minh Nguyen)

* We perform log transformation on price and area, now our model would predict the log of price instead of the price. Our result shows that there is an increase in the R^2 score on training dataset of both models (0.65 to 0.68). However, the R^2 score on testing dataset are stable (0.71). We suggest that this is due to small and biased dataset. We should collect more dataset or perform data interpolation. 
