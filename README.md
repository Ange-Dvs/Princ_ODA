# penguins.ipynb README

## About this project 
The *penguins.ipynb* Jupyter notebook contains the project for the Principal of Data Analytics module. <a target="_blank" href="https://colab.research.google.com/github/Ange-Dvs/Princ_ODA/blob/64f1b6b6e948ce095219ce6dfc2f17c4e7617fcf/penguins.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

It analyses the [Palmer penguins dataset](https://allisonhorst.github.io/palmerpenguins/) looking at the variables within the dataset. The [raw](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/penguins.csv) version of the data was used for the analysis.

## Project summary: 
### Data Analysis & Predictive Analysis:
Pandas and NumPy are used to process and analyse the data from the dataset, allowing filtering and sorting of data based on specified criteria.
These libraries also make it possible to calculate different insights like correlation and standard deviation. 

First the variables in the dataset are broken down to better understand the dataset and information within.  
Then three key questions are addressed in the *penguins.ipynb* notebook with the help of the Pandas and NumPy libraries.  
The spread per island and species inhabiting them will be assessed to see if any patterns are identified.  
The distribution of body mass across the dataset will also be shown and analysed to see if the sex of the penguin has any effect on the distribution.  
Correlation of the body mass and flipper length variables will be calculated, and the species added as a 3rd dimension to see if the species has any impact on correlation. 

### Data Visualisation:
Data Visualisation allows insights gained through the analysis to be represented visually using plots.  
This helps make the findings more accessible with visual aids making it easier to understand patterns and help in facilitating decision making. 

Tabulate is used in the *penguins.ipynb* notebook to create basic tables to show data.
Matplotlib is also used for data visualisation to create and customise plots.  

More information on the methods used in the *penguins.ipynb* notebook from Matplotlib (.pyplot & .ellipse) can be seen below under the "Libraries within Python" section.

## Software used: 
The software used for the creation of this project included VS Code, Python & GitHub.

### Libraries within python: 
Within the program we are importing various external libraries and classes to use throughout the notebook including: 
- Pandas
- Matplotlib.pyplot
- Matplotlib.patches - Ellipse
- NumPy
- Tabulate

#### Pandas:
Pandas[^1] is a library in Python used for data analysis which enables the use of two-dimensional tables called DataFrames.  
Within the *penguins.ipynb* notebook the Pandas library is used to read in the data from the Palmer penguins dataset.  
The following are some methods used throughout the project from Pandas: 
> .corr - used for calculating the correlation coefficient of the variables flipper length and body mass in the dataset.[^2]

> .groupby - allows data to be grouped for analysis based on common values. [^3]  

> .unstack - used with the groups created with groupby() to arrange them in an organised manner. This allows us to create a stacked bar chart to visualise the data of the species per island.[^4] 

>.isna - identifies blank entries in the dataset.  

> .get - uses a defined keyword to search and count how many times the keyword is found in the dataset, if the keyword isn't found a defined value is returned. [^5] 

> .std - used to calculate the standard deviation in the dataset to determine the spread of the values for a variable from the mean. [^6]

#### Matplotlib.pyplot:
The Matplotlib.pyplot library is used mainly for visual representation of the dataset.
This library enables the creation of many types of plots including bar charts, histograms, line plots and scatter plot, all of which are displayed within the *penguins.ipynb* notebook.  
There is a high level of customisation possible with options to switch up the colour,[^7] markers,[^8] labels and titles of the plots.

The following are some methods used throughout the notebook from Matplotlib.pyplot: 

> .scatter - creates scatter plots to visualise the relationship between two variables by plotting markers on a graph where each marker represents an entry in the dataset.[^9]

> .plot - used in the *penguins.ipynb* to create a simple line plots. [^10]

> .hist - creates histogram to represent distribution of values for a variable in the dataset.[^11]

> .subplot - supports the creation of multiple plots in one figure. The number of plots which can be displayed is controlled by values entered for the number of columns and rows required. 

> .xticks & .yticks - offers the ability to change the default tick settings on the x and y axes including the possibility to rotate the labels[^12]  or remove the ticks completely.[^13]

> .xlabel & .ylabel - sets the heading for the axes and allows customisation of the font with the possibility to change the style, font and location of the labels. [^14] 

> .gca - allows you to retrieve the range for the x and y axes for a plot. [^15]

> .xlim & .ylim - used for setting the limit of the x and y axis. This is useful when it's needed to overwrite the default value or range for the axes. [^16]

> .figtext - used for adding text to plots. In *penguins.ipynb* it is used to set super-labels to axes which have a common variable to make the figure less cluttered and easier to read. [^17]

> .figure - is used in *penguins.ipynb* to adjust the size of the figure, to ensure that figures with multiple plots are not overcrowded or distorted and difficult to read. [^18]

#### Matplotlib.patches - Ellipse
The ellipse function [^19] in Matplotlib.patches makes it possible to add an ellipse shape to a plot. 
In *penguins.ipynb* this is used to highlight a cluster of data. 
The width, height, angle and line colour are all configurable allowing the shape to be set to suit the needs of the plot.  

> add_patch - enables shapes to be added to a plot. In *penguins.ipynb* this is used with gca() to ensure the scale for the ellipse shape matches the scale for the original plot. [^20]

#### NumPy
NumPy is used in the *penguins.ipynb* notebook to facilitate calculations on the large amount of data.  When working with datasets NumPy is useful for its ability to handle arrays and possibility to complete mathematical calculation and sorting.[^21]

> .size - used with the groupby() function in *penguins.ipynb* to count the number of entries in the dataset for specified groups i.e. no. per island or no. per species [^22]

> .to_numpy - used to convert the data in the dataset to a NumPy array so that the data can be handled more efficiently for creating plots like histograms [^23]

#### Tabulate
Tabulate makes it possible to create formatted tables to present data from DataFrames and lists in a clear and concise way.  
The table's appearance is customisable, with options to configure if the table has headers and if there are borders between the cells. [^24]

## Author
**by Angela Davis**

***
End

[^1]: https://pandas.pydata.org/docs/user_guide/10min.html#min
[^2]: https://www.geeksforgeeks.org/python-pandas-dataframe-corr/
[^3]: https://www.geeksforgeeks.org/python-pandas-dataframe-groupby/
[^4]: https://medium.com/@anala007/how-to-reshape-your-dataframe-with-pandas-stack-and-unstack-functions-3e2c86edc04a
[^5]: https://www.w3schools.com/python/ref_dictionary_get.asp
[^6]: https://numpy.org/doc/stable/reference/generated/numpy.std.html
[^7]:  https://matplotlib.org/stable/users/explain/colors/colors.html 
[^8]: https://matplotlib.org/2.0.2/api/markers_api.html  
[^9]: https://www.w3schools.com/python/matplotlib_scatter.asp
[^10]: https://www.datacamp.com/tutorial/line-plots-in-matplotlib-with-python
[^11]: https://www.geeksforgeeks.org/matplotlib-pyplot-hist-in-python/
[^12]: https://matplotlib.org/stable/gallery/ticks/ticklabels_rotation.html#sphx-glr-gallery-ticks-ticklabels-rotation-py
[^13]: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.xticks.html#matplotlib-pyplot-xticks
[^14]: https://www.w3schools.com/python/matplotlib_labels.asp   
[^15]: https://realpython.com/python-matplotlib-guide/#stateful-versus-stateless-approaches
[^16]: https://www.geeksforgeeks.org/how-to-set-the-x-and-the-y-limit-in-matplotlib-with-python/
[^17]: https://www.geeksforgeeks.org/matplotlib-pyplot-figtext-in-python/
[^18]: https://www.geeksforgeeks.org/matplotlib-pyplot-figure-in-python/
[^19]: https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Ellipse.html#matplotlib-patches-ellipse
[^20]: https://matplotlib.org/stable/gallery/statistics/confidence_ellipse.html#sphx-glr-gallery-statistics-confidence-ellipse-py
[^21]: https://numpy.org/devdocs/user/whatisnumpy.html
[^22]: https://www.geeksforgeeks.org/numpy-size-function-python/
[^23]: https://www.datacamp.com/tutorial/python-numpy-tutorial
[^24]: https://www.analyticsvidhya.com/blog/2023/12/mastering-tabulate/
