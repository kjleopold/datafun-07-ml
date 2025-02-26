# datafun-07-ml
### Module 7 Project - Intro to Machine Learning
This project is an introduction to machine learning (ML). The goal is to employ a type of supervised learning, simple linear regression, to train a model and use the resulting model to make predictions.  
This project will consist of:
* Building a model
* Making predictions
* Visualize the model
* Publish the insights

## Start a New Project
### 1. Project Setup  
* Create repo named datafun-04-eda in browser with a default README.md.  
* Clone repo to local  
```
git clone (paste repo URL)
```
* Create .gitignore file in root project folder  
 
* Add requirements.txt in root project folder  

    Known dependencies for this project:  
    * jupyterlab
    * numpy
    * pandas
    * pyarrow
    * matplotlib
    * seaborn
    * scipy
    * spacy *- Note: Do not add to requirements.txt, install separately.*
 
### 2. Git add-commit-push  
Push changes from local to GitHub with clear commit message (use this step often).  
```
git add .
git commit -m "Add a message with a clear and descriptive note about what you added or changed."
git push
```

## Create Virtual Environment  
### 1. Create .venv in Version 3.12  
```
py -3.12 -m venv .venv
```
### 2. Activate Virtual Environment  
Always make sure to be in the virtual environment when installing packages and running scripts.  
```
.venv\Scripts\activate
```
### 3. Check Python Version for 3.12
```
py --version
```
### 4. Set VS Code Interpreter
* Open Command Palette: `Ctrl+Shift+P`
* Search "Python: Select Interpreter"
* Chose local .venv option  

## External Dependencies 
### Install necessary dependecies for the project using requirements.txt file.  

```
py -m pip install --upgrade pip setuptools wheel
py -m pip install -r requirements.txt
py -m pip install spacy
```

## Implement 10.16 and 15.4 Sections in Textbook
### Start a New Jupyter Notebook
1. Create a new notebook in your repository named yourname_ml.ipynb.
2. In a Markdown cell at the top of the notebook, add:
    1. The Notebook Title
    2. Author: Name
3. A Clickable Link to your GitHub project repository.
4. In a Python cell just after, add all your import statements, organized following standard conventions. 

### Chart a Straight Line (Part 1)
1. Add a Markdown cell with a second-level heading named Part 1 - Chart a Straight Line
2. Follow the instructions from 10.16 (starting page 414).
3. Use Markdown cells to create section headings
4. Use pandas DataFrames to plot Celsius vs Fahrenheit 

### Predict Avg High Temp in NYC in January (Part 2)
Use Linear Regression on Average High Temperatures in NYC in January. Read these notes before you start:

1. Continue following the instructions from 10.16 (starting page 416).
2. The data is for the average high temperature in January over many years.
3. For example, in 1895, the average high temperature in January was 34.2.
4. We only care about this one series of data: the "average high temp in Jan".
5. There's a lot of stats in the title, and it has confused students. Just think of each value as "the temperature" for that year.
6. Use all of the data available to build a best-fit line (supervised learning). 
7. Use the slope and intercept of the best-fit line to predict a point in the future.

Add a Markdown cell with a second-level heading named Part 2 - Prediction. Use third-level Markdown headings for each section listed below.

1. Section 1 - Data Acquisition
    1. Follow the instructions to load NY City January high temperature from a csv file into a DataFrame.
    2. Recommended: Rather than nyc, name the dataframe nyc_df to reinforce the DataFrame operations.
    3. Recommended: Add all imports to the top of the file, just under the Markdown Introduction. Follow conventions. 
2. Section 2 - Data Inspection
    1. Follow the instructions to view head and tail of the file. 
3. Section 3 - Data Cleaning
    1. Follow the instructions to clean the data. Improve the column names and clean up the date series. 
4. Section 4 - Descriptive Statistics
    1. Set the display precision to 2 decimal places. Use 'display.precision' instead of 'precision' as shown in the text.
    2. Use describe() to calculate basic descriptive statistics for the dataset. 
5. Section 5 - Build the Model
    1. Use the SciPy stats module linregress function to calculate slope and intercept for the best fit line through the data.
    2. Recommended: Add all imports to the top of the file, just under the Markdown Introduction. Follow conventions. 
6. Section 6 - Predict
    1. Use your model to predict the "average high temp in Jan" for the year 2024 (just like they did for 2019).
7. Section 7 - Visualizations
    1. Follow the instructions and use Seaborn to generate a scatter plot with a best fit line.
    2. Set the axes and the y scale as directed

### Predict Avg High Temp in NYC in January (Part 3)
1. Section 1 - Build the Model
    1. Use test_train_split to split the data into parts for training and testing.
    2. Recommended: Add all imports to the top of the file, just under the Markdown Introduction. Follow conventions. 
    3. Check the shape of each data set.
    4. Train the model using Linear Regression Fit. 
    5. View the returned coef_ and intercept_  attributes need for the line equation (y = mx + b)
2. Section 2 - Test the Model
    1. Test the model as directed.
3. Section 3 - Predict 
    1. Use the model to predict the "average high temp in Jan" for the year 2024 (like they did for 2019).
4. Section 3 - Visualizations
    1. Follow the instructions and use Seaborn to generate a scatter plot with a best fit line.
    2. Set the axes and the y scale as directed
    3. Customize your chart and notebook as you like to make your work clear and compelling.

### Add Insights (Part 4)
At the end of your notebook, add a second-level Markdown Heading for Part 4 with some remarks comparing the two methods.

1. Excellent analytical skills need professional communication skills to be of maximum benefit. 
2. The narrative and the way the work is presented is key. 