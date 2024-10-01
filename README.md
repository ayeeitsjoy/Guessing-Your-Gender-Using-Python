# Guessing-Your-Gender-Using-Python
*Fake Data* Insert height (cm), weight (kg), shoe size (european)
VSCODE 
Python 
I started the project by installing pip install scikit-learn inside the terminal in VSCode because I needed the tree module from sklearn. 
The tree module is being used to build a Decision Tree Classifier. Decision Tree is a machine learning model for classification tasks like this one- to predict Male or Female bases on height, weight, and shoe size. It works by splitting data into different groups based on feature values, like a tree-like structure. Each node of a tree, a decision is made about a feature and threshold to split the data on. 
The goal is to spilt data that best seperates the classes (Male or Female) 

----Create a decision tree classifier----
clf = tree.DecicionTreeClassifier()
creates an instance of a decision tree model that will be trained to classify data. 
-----train the model (fitting) 
clf = clf.fit(X,Y) 
X = data trianing features (height, weight, shoe size) 
Y = target labels, Male or Female
This step is where the model learns from the data by finding patterns between Male and Female based on input features I gave. 
During the training the model builds a decision tree by recursively spiltting the data based on the feature that effectively seperates the target classes. 
----Make prediction----
prediction = clf.predict([user_state_list])
After model is trained, it can make predictions successfully. Users can provide new data and the decision tree model uses the learned patterns to classify the input as Male or Female
----Change string to integar----
user_state_list = list(map(int, user_state.split(',')))
This code takes the user's input, splits it into separate values, turns those values into real numbers, and then stores them in a list for the model to understand
