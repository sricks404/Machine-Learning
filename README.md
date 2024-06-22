# Machine Learning

Hello Everyone !
<br>

Welcome to my <b>`Machine Learning`</b> repository. Here, I will talk about some graduate-level concepts, algorithms, tools and frameworks related to Machine Learning, which bolster the foundation of research and development, especially in the field of <u>[Data Science](https://www.ibm.com/topics/data-science)</u>.
<br>

> NOTE : The programming language used here (i.e., in every jupyter notebook) is **Python**, as it is the most widely used in the industry.

<br>

Let us now go over the notebooks mentioned here. <i>For your information, the <u>sequence</u> below is organized by increasing levels of complexity of the work done in each notebook.</i>
<br>

### **[Python - Data Analysis - Basics](https://github.com/sricks404/Machine-Learning/blob/main/Python%20-%20Daya%20Analysis%20-%20Basics.ipynb)** 👇<br>

Python, *being the medium of conversation between us and the machine learning models*, demands solid foundation, as a pre-requisite,  in numerous programming concepts - such as 🔻
- Data structures (like `Lists`, `Dictionaries`, `Sets`, `Tuples`, etc.)
- Data types 
- Functions
- Logic / Control Flow
- Working with External Libraries
- 
- ... <i><b>and the list goes on !!!</b></i>
<br>

This notebook, in particular, should give you a good kickstart on clearing up your <i>Python</i> basics. Here, you will also be going to play with the functions (<i>methods</i>) of <b>[Numpy](https://numpy.org/doc/stable/index.html#)</b> - <i>"The fundamental package for scientific computing in Python"</i>, which shall give you the initial taste of <b>[Data Pre-processing](https://towardsdatascience.com/introduction-to-data-preprocessing-in-machine-learning-a9fa83a5dc9d)</b>. You will also experience the *"ease-of-formulating"* of complex mathematical functions using inbuilt <i>numpy</i> objects and methods. 
<br>

Next up, you will have **[Pandas](https://pandas.pydata.org/)** - <i>"A data analysis and manipulation tool,  built on top of Python programming language."</i> You will explore how to <i>"talk"</i> to a dataset. There are numerous inbuilt datasets in the Pandas library, but the  majority of the times, you will be working on external datasets - <u>downloaded</u> *OR* <u>extracted</u> from the web. Pandas also allows you for intermediate level data pre-processing like <i>String to Categorical datatype conversion, finding the min/max. value of an attribute, attribute drop / rename, etc.</i>
<br>

Possessing data and pre-preprocessing is just one of step of the many steps in data analysis. On later stage, you need to unravel <i>"What the data is conveying"</i>. And, for that, visual representation of the data is an added advantage. Here comes <b>[Matplotlib](https://matplotlib.org/)</b> - *"Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. It is widely used in data science, machine learning, and scientific computing to generate plots and graphs for data analysis and presentation."*  Whether it's a [heat map](https://matplotlib.org/stable/gallery/images_contours_and_fields/image_annotated_heatmap.html), [line plot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html), [scatter plot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html), [bar plot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html), matplotlib covers it all. We have another visualization library called <b>[Seaborn](https://seaborn.pydata.org/#)</b> - but here the question comes - ***"Why having 2 libraries for the same purpose ?"** - Seaborn complements Matplotlib by simplifying the creation of visually appealing statistical graphics with a more intuitive syntax and built-in themes. It provides specialized functions for complex plots like heatmaps and regression plots, integrates seamlessly with Pandas Dataframes, and automates many design aspects, reducing the need for extensive coding. This makes Seaborn ideal for quickly generating attractive and informative visualizations.* 

**[Scikit-Learn](https://scikit-learn.org/)** - *"is an open-source machine learning library for the Python programming language."* Whether it's a [classification](https://www.geeksforgeeks.org/getting-started-with-classification/) problem, dealing with a [regression](https://www.geeksforgeeks.org/regression-in-machine-learning/) dataset or need to put a [clustering](https://www.geeksforgeeks.org/clustering-in-machine-learning/) algorithm to work, scikit-learn contains a whole lot of varieties in algorithms to work with for different purpose and also provide data pre-processing functionalities (like splitting the data into *training* and *testing* components). In this notebook you will see the usage of **[Logistic Regression](https://www.geeksforgeeks.org/understanding-logistic-regression/)** algorithm  to predict the *"species"* of penguins using all the features in the **[Penguin](https://www.kaggle.com/code/parulpandey/penguin-dataset-the-new-iris)** dataset.

Lastly, you will have **[Optuna](https://optuna.org/)** - *"Optuna is an open-source software framework for hyperparameter optimization, written in Python. It is designed to be efficient, flexible, and easy to integrate with existing machine learning libraries and frameworks. Optuna aims to automate the process of hyperparameter tuning, which is crucial for improving the performance of machine learning models."* Here, Optuna is used to optimize hyperparameters like `C` (regularization strength),  `solver` (optimization algorithm) and `max_iter` (maximum number of iterations) for Logistic Regression models, aiming to improve performance metrics such as accuracy.
<br>
<br>

### **[Python - Data Analysis and Preprocessing](https://github.com/sricks404/Machine-Learning/blob/main/Python%20-%20Data%20Analysis%20%26%20Preprocessing.ipynb) 👇**
<br>

Now that you are done grasping some knowledge about how to use some of the essential python libraries, it's time to hit the playground to play with datasets. 

> NOTE : The notebooks were run in `google colab environment`. If you want to try the same, just copy paste the below code in the starting cell of your notebook 🔻<br>

~~~
from google.colab import drive
drive.mount('/content/drive')
~~~
<br>

In this notebook, one of the most famous datasets has been used for the purpose of data analysis and preprocessing - <b>[penguins dataset](https://www.kaggle.com/code/parulpandey/penguin-dataset-the-new-iris)</b><br>

Data Preprocessing steps include 🔻<br>

- Handling Missing Entries<br>
- Handling Mismatched String Formats<br>
- Handling Outliers<br>
- Detecting and Managing Outliers within the dataset<br>
- Identifying Uncorrelated / Unrelated Features<br>
- Converting Features with String Datatypes to Categorical<br>
- Normalizing Non-Categorical Features<br>

> NOTE : It's always a good practice to export / save the preprocessed data because many a times, you shall be building your machine learning models in a separate notebook. As data preprocessing, if done on a huge dataset, consumes a significant amount of compute resources, thus ,a separate session shall be required for model building, training and evaluation.

<br>


### **[Data Analysis - Logistic Regression](https://github.com/sricks404/Machine-Learning/blob/main/Data%20Analysis%20-%20Logistic%20Regression.ipynb) 👇**<br>

Here, you will be encountering one of the first machine learning algorithm used in this repo - [logistic regression](https://www.geeksforgeeks.org/understanding-logistic-regression/). The dataset used is the preprocessed version of `penguins` dataset, whose original version was used for data analysis and preprocessing in the previous notebook.<br>

Below are the steps taken for training and evaluation of logistic regression model 🔻<br>

- Importing required libraries
- Loading the preprocessed dataset
- Choosing the target feature <b>(`y`)</b>
- Creating the data matrices for input data <b>(`X`)</b> and target data <b>(`y`)</b>
- Dividing the dataset into training and testing components
- Printing the shapes of the divided data components to confirm successful division
- Designing and implementing "logistic regression" model (according to the underlying mathematical formula and functions)
- Model Training
- Saving the weights of the model, which gave the  highest accuracy <i>(The evaluation metric can be changed according to your needs - especially te type of algorithm you chose and the type of problem you are solving)</i>
- Making prediction on <i>test dataset</i>
- Plotting the loss graph and printing out the loss values over each iteration<br>

> NOTE : When you try to save the weights of the model (either as a pickle `(.pkl)` file or as  HDF5 `(.h5)` file), make sure it can be successfully loaded again, say, for <i>model deployment</i>.

<br>


### **[Data Analysis - Linear Regression](https://github.com/sricks404/Machine-Learning/blob/main/Data%20Analysis%20-%20Linear%20Regression.ipynb) 👇**<br>








