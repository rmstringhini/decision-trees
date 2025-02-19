# **Decision Trees**

* Decision Tree is a supervised machine learning algorithm used for both classification and regression which mimics human decision-making by splitting data into branches based on feature values, leading to a decision.

Key concepts:

**1) Structure of a Decision Tree**

- A decision tree consists of:
  - **Root Node**: The starting point of the tree where the first split occurs;
  - **Internal Nodes (Decision Nodes)**: Nodes where decisions are made based on feature values;
  - **Leaf Nodes (Terminal Nodes)**: Nodes representing the final decision (class label or numerical value);

- How a decision tree works:

  1- Select the best feature to split the data;

  2- Create a decision node and split the dataset;

  3- Repeat recursively for each subset until:
  
  - All data points in a node belong to the same class (for classification);
  - A stopping criterion (e.g., max depth, min samples per node) is met.

**2) Splitting Criteria in Decision Trees**

- The decision tree selects the best feature to split based on impurity measure:

A) For classification:
  - **Gini impurity**: measures how often a randomly chosen element would be incorrectly classified:
    
  $ Gini = 1 - \sum p_{i}^{2}$

  where $p_i$ is the probability of class $i$;

  - **Entropy**: measures the uncertainty in the dataset:

  $ Entropy = -\sum p_i \log_2(p_i)$

B) For regression:
  - **Mean Squared Error (MSE)**: measures variance within a node:

  $MSE = \frac{1}{n} \sum (y_i - \bar{y})^2$

  where $\bar{y}$ is the mean target value in a node.


  ![decision-trees](https://github.com/user-attachments/assets/0c173001-f9ba-48f5-ab37-e9c972ba2506)
