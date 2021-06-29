# aws_machine_learning_log
Learning Log + Scratch pad for AWS Machine Learning Foundation Udacity

12k on Foundation
425 possible Nano Degree for top performers! 
https://aws.amazon.com/blogs/machine-learning/ 

## Course Overview
1. Lession 1: Introduction to course. 
2. Lesson 2: Introduction to Machine Learning – In this lesson, you will learn the fundamentals of supervised and unsupervised machine learning, including the process steps of solving machine learning problems, and explore several examples.
3. Lesson 3: Machine Learning with AWS – In this lesson, you will learn about advanced machine learning techniques such as generative AI, reinforcement learning, and computer vision. You will also learn how to train these models with AWS AI/ML services.
4. Lesson 4: Software Engineering Practices, part 1 – In this lesson, you will learn how to write well-documented, modularized code.
5. Lesson 5: Software Engineering Practices, part 2 – In this lesson, you will learn how to test your code and log best practices.
6. Lesson 6: Object-Oriented Programming – In this lesson, you will learn about this programming style and prepare to write your own Python package.

## End of Course

1. Explain machine learning and the types of questions machine learning can help to solve.
2. Explain what machine learning solutions AWS offers and how AWS AI devices put machine learning in the hands of every developer.
3. Apply software engineering principles of modular code, code efficiency, refactoring, documentation, and version control to data science.
4. Apply software engineering principles of testing code, logging, and conducting code reviews to data science.
5. Implement the basic principles of object-oriented programming to build a Python package.

## Log

29/06/2021
1. Starting Udacity course.
2. Created AWS + Joined Slack community. 
3. Worked through welcome to AWS Machine Learning Lesson 1.
4. Watch the youtube stream for the course. 
5. Welcoem to Machine Learning - Lesson 2 Start

### Lesson 2 
What is Machine Learning  
Steps in Machine Learning  
Real world examples  
 
#### What is Machine Learning
ML is a type of AI, automatically learn without being programmed, patterns and predictions
supervised learning - every training sample has a matching label or output label - predictions - sale price of house or image classification. 
unsupervised no labels. 
Inspect data to find patterns then humans use patterns to make insights. 
Reinforcement learning in what actions to take in situations to get max rewards. (Like a pet) 
 
Analyse problems and programs solutions - time taking and might be undoable. Because of edge cases. 
Machine learning - Models - Model training algorithm - predict outcomes that aren't partt of the data set used to train it, pattern matching that the problem solver would traditionally do. Flexiblity of the model is the key here. 

#### Components of Machine Learning

3 Primary components 
Machine Learning Model, Model training alghorithm, Model inference Algorithm.
Clay -> Raw -> Fired. 
Clay - Can be modelled into many different forms and purposes. 
Block of code or framework. For Example Linear regression model example. 
People attenting college based on cost of application eg. 

Raw Teapot - Inspect and analyse Clay and look at what to change to make it more like a teapot. gentle changes to model parameters to achieve goals. 
Determine what changes need to be made. 
Processes data and compares against a goal and makes small changes. Repeated step. 

Teapot - Ready for the real world. 
Generate preditions. 
Model inference 
 
#### Completed Quiz

### Introduction to the Five Machine Learning Steps
Common workflow.

1. Define the Problem 
2. Build the Dataset 
3. Train the Model
4. Evaluate the Modle
5. Use the Model 

These steps are iterative. In practice, that means that at each step along the process, you review how the process is going. Are things operating as you expected? If not, go back and revisit your current step or previous steps to try and identify the breakdown.

#### Step 1: Define the Problem 

1. Define a very specific task 
Has to be a keyed in task for example, would offering a service at price point x increase sales rather than broad how do I increase sales. 

Examples:
“Does adding a $1.00 charge for sprinkles on a hot fudge sundae increase the sales of hot fudge sundaes?”
“Does adding a $0.50 charge for organic flavors in your snow cone increase the sales of snow cones?”

2. Identify the machine learning task we might use to solve this problem.

All models take data as input, but output varies on task they are designed to solve. 
Often we used the kind of data required to train a model as part of defining a machine learning task.

Supervised + Unsupervised. 

Predicting the number of snow cones sold based on the temperatures is an example of supervised learning. Since we have both temperature and numbers of snowcone sold. Already contains the solution. 
Labeling a picture with a object in it would be unsupervised learning. Microgenres in books would be another example. 

Clustering -  Unsupervised learning task that helps to determine if there are any naturally occurring groupings in the data.

Supervised learning - Categorical label (Classification) - Continous Label (Regression) 
Unsupervised Learning - Clustering.

#### Step 2: Build a Dataset

1. Data collection - Does the data you've collected match the machine learning task and problem you have defined?
2. Data inspection
- Outliers
- Missing or incomplete values
- Data that needs to be transformed or preprocessed so it's in the correct format to be used by your model
4. Summary Statistics - Insight into the scope, scale, and shape of the dataset
5. Data Visualization - You can use data visualization to see outliers and trends in your data and to help stakeholders understand your data.

Impute is a common term referring to different statistical tools which can be used to calculate missing values from your dataset.

#### Step 3: Model Training 

1. Split dataset - 80% Training Dataset 20% Test set (Model evaluation stage) Validation Data
2. Iteratively update model parameters to minimize some loss function - Setting to change how the model behaves biases - Regression changes the shape of the line. Loss function is the model's distance from the score. Seek to minimise loss function. 
- Feed the training data into the model.
- Compute the loss function on the results.
- Update the model parameters in a direction that reduces loss.
- You continue to cycle through these steps until you reach a predefined stop condition. 

1. Practitioners often use machine learning frameworks that already have working implementations of models and model training algorithms. You could implement these from scratch, but you probably won't need to do so unless you’re developing new models or algorithms.
2. Practitioners use a process called model selection to determine which model or models to use. The list of established models is constantly growing, and even seasoned machine learning practitioners may try many different types of models while solving a problem with machine learning.
3. Hyperparameters are settings on the model which are not changed during training but can affect how quickly or how reliably the model trains, such as the number of clusters the model should identify.
4. Be prepared to iterate.

##### Extra reading 

Linear models
One of the most common models covered in introductory coursework, linear models simply describe the relationship between a set of input numbers and a set of output numbers through a linear function (think of y = mx + b or a line on a x vs y chart).

Classification tasks often use a strongly related logistic model, which adds an additional transformation mapping the output of the linear function to the range [0, 1], interpreted as “probability of being in the target class.” Linear models are fast to train and give you a great baseline against which to compare more complex models. A lot of media buzz is given to more complex models, but for most new problems, consider starting with a simple model.

Tree-based models
Tree-based models are probably the second most common model type covered in introductory coursework. They learn to categorize or regress by building an extremely large structure of nested if/else blocks, splitting the world into different regions at each if/else block. Training determines exactly where these splits happen and what value is assigned at each leaf region.

For example, if you’re trying to determine if a light sensor is in sunlight or shadow, you might train tree of depth 1 with the final learned configuration being something like if (sensor_value > 0.698), then return 1; else return 0;. The tree-based model XGBoost is commonly used as an off-the-shelf implementation for this kind of model and includes enhancements beyond what is discussed here. Try tree-based models to quickly get a baseline before moving on to more complex models.

Deep learning models
Extremely popular and powerful, deep learning is a modern approach based around a conceptual model of how the human brain functions. The model (also called a neural network) is composed of collections of neurons (very simple computational units) connected together by weights (mathematical representations of how much information to allow to flow from one neuron to the next). The process of training involves finding values for each weight.

Various neural network structures have been determined for modeling different kinds of problems or processing different kinds of data.

#### Step 4: Model Evaluation (How well the model works) 

https://aws.amazon.com/blogs/machine-learning/making-accurate-energy-consumption-predictions-with-amazon-forecast/

Not a one and done process. 

Model accuracy - How often your model is correct - Classification. 

Metrics
- Recall: Fraction of relevant instances that were retrieved.
- Precision: Fraction of relevant instances among the retrieved instances
- Log Loss: Seeks to calculate how uncertain your model is about the predictions it is generating.
- Mean Absolute Error:  Absolute error refers to the magnitude of difference between the prediction of an observation and the true value of that observation.
- Hinge Loss: How close a binary classification is with notion of a margin.
- R2: proportion of the variance for a dependent variable, actual and observed probability distribution.
- KL Divergence: difference between an actual and observed probability distribution.
- F1 Score: F1 score conveys the balance between the precision and the recall. 
- Quantile Loss:  A quantile is the value below which a fraction of observations in a group falls. For example, a prediction for quantile 0.9 should over-predict 90% of the times.




