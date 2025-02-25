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
- Create repo named datafun-04-eda in browser with a default README.md.  
- Clone repo to local  
```
git clone (paste repo URL)
```
- Create .gitignore file in root project folder  
 
- Add requirements.txt in root project folder  
Known dependencies for this project:  
* jupyterlab
* numpy
* pandas
* pyarrow
* matplotlib
* seaborn
* scipy
 

### 2. Git add-commit-push  
Push changes from local to GitHub with clear commit message (use this step often).  
```
git add .
git commit -m "Add a message with a clear and descriptive note about what you added or changed."
git push
```

## Create Virtual Environment  
### 1. Create `.venv`
```
py -m venv .venv
```
### 2. Activate Virtual Environment  
Always make sure to be in the virtual environment when installing packages and running scripts.  
```
.venv\Scripts\activate
```
### 3. Set VS Code Interpreter
* Open Command Palette: `Ctrl+Shift+P`
* Search "Python: Select Interpreter"
* Chose local .venv option  

## External Dependencies 
### Install necessary dependecies for the project using requirements.txt file.  

```
py -m pip install --upgrade pip setuptools wheel
py -m pip install -r requirements.txt
```