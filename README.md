# Archived project. No maintenance.
This project is not maintained anymore. You may fork and make your changes, freely.

# Plotting time-resolved data (from femtosecond to millisecond) with linear - logarithmic axis.

This project provides codes for plotting time-resolved data with linear-logarithmic axis in python. 

## About the source code

You will see in the repo that there are two scripts. 

This one `Plot_linlogtrace_from_csv.ipynb` can import from .csv file, whereas the other script `Plot_linlogtrace_from_matfile.ipynb` can import from .mat file. Except this, they are both doing the same thing. Choose one you like to work with. At the end of every script, there is a preview of plot. 

## Background

Time-resolved spectroscopy is a common method to reveal time-dependent events in nature. Depending on the method, time-axis may involve a very wide time-scale which is difficult to plot it linear. If it is plotted linear, then fast events will be invisible. If it is plotted logarithmic, then time-axis has to start from a value which is bigger than zero (0). In order to show all the time-scale in one axis, the plot has to be divided; fast time-scale would be plotted in linear, slow time-scale would be plotted in logarithmic.

In our case, where femtosecond lasers are used, time axis starts from femtoseconds (10<sup>-15</sup> seconds) and may end in milliseconds (10<sup>-3</sup> seconds). This needs to be plotted in either logarithmic or in combination of linear-logarithmic. Since the time axis includes "time zero" which is the moment of excitation, it is not possible to draw this moment with only logarithmic scale. What we need here is the combination of linear-logarithmic scale for time-axis. 

### Prerequisites

* [Python](https://www.python.org/) (latest version if possible)
The given codes are developed in Python. For this you need to have Python in your computer. An easy way to download Python is to use [Anaconda](https://www.anaconda.com).
* [Matplotlib](https://matplotlib.org) (A plotting package for Python).
* [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/). Web based user interface to run the code. It is an integrated environment. This will make the life easier for the enduser to edit/run python codes and visualize the plots. Check one of the codes with .ipynb extension in the repository. 

## Built With

* [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/)

## Acknowledgment

Thanks to Patrick Konold, he gave the idea for this project.
