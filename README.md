# Building-Your-Own-Prediction-Model
this repository includes the concept of ML classification and techniques for evaluation. 
ALso learned in depth about decision Trees
Also created a model to predict student performance.

Requirement:
knowledege on python and especially familiar with Python's Library
knowledge about classification problem
knowledge anout Decision Trees , Entropy and Information gain
datasets handling in python

platform:
Any python workshop i prefer Jupyter Notebook

Explanation:
we're going to use decision trees to predict student performance using the
students, past performance data. We'll use the student performance dataset, which is
available on the UC Irvine machine learning repository at https://archive.ics.uci.edu/ml/datasets/student+performance 

Our final goal is to predict whether the student has
passed or failed. The dataset contains the data of about 649 students, with and 30 attributes
for each student. The attributes formed are mixed categorically b word and phrase, and
numeric attributes. These mixed attributes cause a small problem that needs to be fixed. We
will need to convert those word and phrase attributes into numbers.

We import the dataset (student-por.csv), which comes with semicolons instead of
commas; hence, we mention the separators as semicolons. To cross verify, we will find the
number of rows in the dataset. Using the length variable, we can see that there are 
rows.

Next we add columns for pass and fail. The data in these columns would contain 1 or 0,
where 1 means pass and 0 means fail. We are going to do that by computing with every
row what the sum of the test scores would be. This will be calculated as if the sum of three
score is greater than or equal to 35, 1 is given to the student and failing to that rule 0 is
given to the student.

As mentioned before, some of these columns are words or phrases, such as Mjob, Fjob,
internet, and romantic. These columns need to be converted into numbers, which can be
done using the HFU@EVNNJFT function, which is a Pandas feature, and we need to mention
which columns are the ones that we want to turn into numeric form.

then we suffle the datasets to avoid overfiting on 80/20 basis.
we start building the decision tree using the DecisionTreeClassifier function
from the scikit-learn package, which is a class capable of performing multi-class
classification on a dataset. Here we will use the entropy or information gain metric to
decide when to split.

