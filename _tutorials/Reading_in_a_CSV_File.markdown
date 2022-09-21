---
layout: page
title: Reading a CSV with Python
permalink:/Reading a CSV with Python/
---


This lab will follow a step-by-step guide on how to read a CSV file that you have stored on your computer or server. 

The file's location on your computer or server is essential because if you move the file, you will need to point Python to the file's position. 

Download the [Alcohol Consumption by Country](https://www.kaggle.com/datasets/pralabhpoudel/alcohol-consumption-by-country) CSV file from Kaggle and save it to your desktop. 

We will be using Visual Studio Code to run this example. Please download and set up [Visual Studio Code](https://code.visualstudio.com/Download) on your computer. 

After you install Visual Studio Code, add the [Python extension.](https://code.visualstudio.com/docs/python/python-tutorial)

### Import the Pandas Library 

    `import pandas as pd`

This statement assigns an alias to the ***pandas*** library so you don't have to keep typing out the word as you code. 

### Assign a variable to the CSV file

Assigning a variable name to your file tells Python what the file location should be called. 

    `url='C:/Users/Maryam/Desktop/consumption.csv'`
### Read the CSV file 

**Cons** is also a variable name, but in this case, it has been assigned as the name of the project you are working on. 

    `cons = pd.read_csv(url,  header=0, na_filter=False)`




