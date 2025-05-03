1. How does a decision tree work?
Think of a decision tree like a flowchart. It starts with a question (like “Is age > 50?”) and branches out based on answers, splitting the data into smaller groups each time. The goal is to keep splitting until each group is as “pure” as possible—meaning it mostly contains one class (like “has heart disease” or “doesn’t”).

2. What are entropy and information gain?
Entropy measures uncertainty or disorder in the data—kind of like how mixed up it is. Information gain tells us how much better we get at classifying things if we make a certain split. In short, we look for the question that gives us the biggest improvement (highest information gain) in making accurate predictions.

3. Why is a random forest better than a single tree?
A single decision tree can be too confident and easily fooled by noise. A random forest builds lots of decision trees on different parts of the data and averages their results. This "wisdom of the crowd" approach tends to give more reliable, accurate predictions and is less likely to overfit.

4. What is overfitting, and how do you prevent it?
Overfitting is like memorizing instead of understanding—it means the model learns the training data too well, including its noise, and performs poorly on new data. To prevent it, we can limit the tree’s depth, use pruning, or switch to methods like random forests which naturally reduce overfitting.

5. What is bagging?
Bagging, short for “Bootstrap Aggregating,” is a technique where we create multiple versions of a dataset by randomly sampling with replacement, train a model (like a decision tree) on each version, and then average the results. It helps reduce variance and makes models more stable and accurate.

6. How do you visualize a decision tree?
In Python, you can use plot_tree from scikit-learn. It draws the entire tree with questions, thresholds, and predicted outcomes at each node—like a map showing how decisions are made step-by-step.

7. How do you interpret feature importance?
Feature importance tells you which features (like cholesterol or age) matter most in making predictions. In decision trees and random forests, it's calculated based on how much each feature helps reduce uncertainty (entropy) across all the splits where it's used.

8. What are the pros and cons of random forests?
Pros:
Great accuracy and generalization
Handles both classification and regression
Works well with missing data and unscaled inputs
Resistant to overfitting

Cons:
Slower to train and predict than a single tree
Less interpretable—harder to explain why a specific decision was made
Can use more memory

