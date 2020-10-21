# cs_build
Implementing CART Decision Tree Algorithm 

To use, import the good_tree.py file,

Then replace your classifier of choice in your pipeline with my DecisionTree

Example:

import category_encoders as ce
# import my python file here
from good_tree import DecisionTreeClassifier
from sklearn.impute import SimpleImputer
from sklearn.pipeline import make_pipeline


# Make pipeline!
pipeline = make_pipeline(
    ce.OrdinalEncoder(), 
    SimpleImputer(strategy='most_frequent'), 
    DecisionTreeClassifier(max_depth=1) 
                       )
                       
