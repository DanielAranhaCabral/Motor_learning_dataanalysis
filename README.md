# Data processing and Analysis on Motor Performance
Processing Raw Performance Data
Daniel Cabral
2022-07-14
The following code was written in Python. To run the code in R, it is necessary to install the package “reticulate” and run the function install_cond(path = “Whatever path you want”).
Note that we used a custom LabVIEW program (Neumann and Thomas, 2008) to measure the distance of the ball from the target along the x and y axes. The code below imports these distances from each participant for every condition and concatenates them into one data frame. Next, the code calculates radial error and bivariate variable error for each trial. The resultant data frame can then be imported into an R Markdown file for statistical analyses.
The custom LabView program and the x- and y-axis data it yielded as well as the R Markdown file for statistical analyses can be found in supplementary materials.
Uploading packages import numpy as np import pandas as pd import glob
Here, we are using data from pretest. You can easily change the path to where the data from posttests and acquisition are. You may also need to change some variables’ names accordingly.
