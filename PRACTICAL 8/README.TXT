1. Data Collection
Download the Pima Indians Diabetes Dataset from Kaggle.
The dataset contains medical predictor variables (features) and a target variable (Outcome).

2. Data Understanding
The dataset includes the following independent variables (features):
Pregnancies
Glucose
BloodPressure
SkinThickness
Insulin
BMI
DiabetesPedigreeFunction
Age
The dependent variable (target) is:
Outcome → (0 = No Diabetes, 1 = Diabetes)
This classification problem aims to predict whether a person is diabetic.

3. Feature Selection
Feature selection means identifying which columns will be used to train the model.
Independent Variables (X):
All medical measurements except Outcome.
Dependent Variable (y):
Outcome — because this is what we want to classify.
Thus, we divide the dataset into:
X (input features)
y (output/label)

4. Data Splitting
To evaluate model performance fairly:
The dataset is split into:
Training Set (usually 80%)
Testing Set (usually 20%)
Reason:
Training set is used to build the decision tree.
Testing set is used to evaluate the final model.

5. Decision Tree Construction
A Decision Tree Classifier learns patterns by repeatedly splitting the dataset based on features.
Two common criteria for splitting:
Entropy (Information Gain)
Gini Index
A split is chosen so that the resulting groups become pure (more similar class values).

6. Visualization of the Tree
Decision trees can be visualized as:
Nodes (decision points)
Branches (paths)
Leaves (final class outputs)
Visualization helps understand:
Which feature the tree chooses as the root node
What conditions split the dataset
Typically, in this dataset, Glucose becomes the root node because it provides the best separation.

7. Calculating Entropy, Information Gain & Gini Index
These calculations support why the tree chose the root node.

8. Choosing the Root Node
A decision tree chooses the root node based on:
Highest Information Gain (if criterion = entropy)
Lowest Gini Impurity (if criterion = gini)
In the Pima Indian Diabetes dataset:
Glucose usually becomes the root node because it best separates diabetic and non-diabetic individuals.
Thus, it has:
Highest reduction in entropy
Lowest Gini impurity
Highest information gain

9. Model Evaluation
After training:
Predict on the test set
Compare predictions vs actual values
Evaluate using:
Accuracy
Confusion Matrix
Precision / Recall
F1 Score
This tells how well the decision tree performs.
