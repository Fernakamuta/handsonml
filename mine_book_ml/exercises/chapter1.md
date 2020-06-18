# 1) How would you define machine learning?
- Machine Learning is about building a system that can learn from data. Learning means getting better at some task, given some performance measure.

# 2) Can you name four types of problems where it shines?
- Estimating sentiment by a text.
- Finding spams emails.
- Estimating the probability of inadimplence of a retail.
- Estimating the best route of a car trip. 

# 3) What's a labeled training set?
- A labeled training set is a set that contains the variable we want to predict in a supervised problem. 

# 4) What are the two most common supervised tasks?
- Classification and regression.

# 5) Can you name four common unsupervised tasks?
- Clustering, Visualization, Dimensionality Reduction, Association rule learning 

# 6) What type of machine learning algorithm would you use to allow a robot to walk in  various unknown terrants?
- Reinforcement learning.

# 7) What type of algorithm would you use to segment your customers profiles?
- K-Means.

# 8) Would you frame the problem of spam detection as a supervised learning problem or an unsupervised learning problem?
- Supervised Problem. 

# 9) What is an online learning system?
- This is a type of model that is updated automatically that new inputs enter the platform.

# 10) What is out-of-core learning?
-  Out-of-core algorithms can handle vast quantities of data that cannot fit in a computer’s main memory. An out-of-core learning algorithm chops the data into mini-batches and uses online learning techniques to learn from these mini-batches.

# 11) What type of algorithm relies on a similarity measure to make predictions?
- An instance-based learning system learns the training data by heart; then, when given a new instance, it uses a similarity measure to find the most similar learned instances and uses them to make predictions.

# 12) What is the difference between a model parameter and a learning algorithm's hyperparameter?
- A model has one or more model parameters that determine what it will predict given a new instance (e.g., the slope of a linear model). A learning algorithm tries to find optimal values for these parameters such that the model generalizes well to new instances. A hyperparameter is a parameter of the learning algorithm itself, not of the model (e.g., the amount of regularization to apply).

# 13) What do model-based learning algorithms search for? What is the most common strategy they use to succeed? How do they make predictions?
- Model-based learning algorithms search for an optimal value for the model parameters such that the model will generalize well to new instances. We usually train such systems by minimizing a cost function that measures how bad the system is at making predictions on the training data, plus a penalty for model complexity if the model is regularized. To make predictions, we feed the new instance’s features into the model’s prediction function, using the parameter values found by the learning algorithm.

# 14) Can you name four of the main challenges in machine learning?
- Insufficient data.
- Bad quality data.
- Non-representative data and uninformative features.
- Simple models that underfit the training data.
- Very complex models that overfit the training data.

# 15) If your model performs great on the training data but generalizes poorly to new instances, what is happening? can you name three possible solutions?
- If a model performs great on the training data but generalizes poorly to new instances, the model is likely overfitting the training data (or we got extremely lucky on the training data). Possible solutions to overfitting are getting more data, simplifying the model (selecting a simpler algorithm, reducing the number of parameters or features used, or regularizing the model), or reducing the noise in the training data.

# 16) Whats is a test set and why would you want to use it?
- A test set is used to estimate the generalization error that a model will make on new instances, before the model is launched in production.

# 17) What is the purpose of a validation set?
- A validation set is used to compare models. It makes it possible to select the best model and tune the hyperparameters.

# 18) What can go wrong if you tune hyperparameters using the test set?
- If you tune hyperparameters using the test set, you risk overfitting the test set, and the generalization error you measure will be optimistic (you may launch a model that performs worse than you expect).

# 19) What is cross-validation and why would you prefer it to a validation set?
- Cross-validation is a technique that makes it possible to compare models (for model selection and hyperparameter tuning) without the need for a separate validation set. This saves precious training data.