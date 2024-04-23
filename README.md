# penguins.ipynb README

## About this project 
The *penguins.ipynb* Jupyter notebook contains the project for the Principal of Data Analytics module. 

The project analyses the [Palmers penguin dataset](https://allisonhorst.github.io/palmerpenguins/) looking at the variables within the dataset. The [raw](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/penguins.csv) version of the data was used for the project.

The notebook utilizes plots such as bar charts, histograms and scatter plots to visulise the data contained within the dataset.

Two of the variables in the dataset will also be analysed and the correlation discussed. For the purpose of this project we will look at the correlation between flipper length and body mass of the penguins.

## Software used: 
This project was created using VS Code, python & GitHub.

### Libaries within python: 
Within the python code we are importing 3 modules at the beginning of the notebook to use throughout.
#### pandas:
Within the *penguins.ipynb* project the pandas library is used to read in the data from the palmers penguins dataset. 
The corr() method is used in calculating the correlation coefficient of the variables flipper length and body mass in the dataset.[^1]
groupby() method
unstack() - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.unstack.html#pandas.DataFrame.unstack
.isna().sum() 
.get()
.std()

https://aaltoscicomp.github.io/python-for-scicomp/pandas/
https://pandas.pydata.org/docs/user_guide/10min.html#min
https://www.geeksforgeeks.org/python-pandas-dataframe-groupby/

#### matplotlib.pyplot:
The matplotlib.pyplot libray is used mainly for visual representation of dataset.
The use of this library enables the user to create many types of plots including bar charts, histograms, line plots and scatter plot, all of which are displayed within the *penguins.ipynb* project.  
With matplotlib.pyplot the user also has the possibility to save the graphs created by the program. 
The user is also enabled to customize the charts to their liking with options to switch up the colour,[^2] markers,[^3] labels and titles[^4] of the plots.
title() https://matplotlib.org/stable/gallery/text_labels_and_annotations/titles_demo.html
axis label rotation - https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.xticks.html#matplotlib-pyplot-xticks
drawing an ellipse - https://matplotlib.org/stable/gallery/shapes_and_collections/ellipse_demo.html#ellipse-demo
Ellipse - https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Ellipse.html#matplotlib-patches-ellipse

https://www.datacamp.com/tutorial/line-plots-in-matplotlib-with-python

#### numpy
Numpy is a widely known Python libary in part for it's ability to facilitates basic and advanced arithmetic operations on large numbers of data and also for it's random number generating functionality.  When working with datasets numpy is useful due to it's ability to handle arrays and swiftly perform operations on them; like mathematical calution and sorting.[^5]  
size method()
.to_numpy()


https://www.geeksforgeeks.org/numpy-size-function-python/

#### tabulate



## Project run through

### Customization of the plots

## Supporting reading material:
https://archive.ics.uci.edu/dataset/690/palmer+penguins-3
https://allisonhorst.github.io/palmerpenguins/      
https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.corr.html
https://github.com/hackergrrl/art-of-readme

## Author
**by Angela Davis**

***
End

[^1]: https://www.geeksforgeeks.org/python-pandas-dataframe-corr/
[^2]: https://matplotlib.org/stable/users/explain/colors/colors.html  
[^3]: https://matplotlib.org/2.0.2/api/markers_api.html  
[^4]: https://www.w3schools.com/python/matplotlib_labels.asp  
[^5]: https://numpy.org/devdocs/user/