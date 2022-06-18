##  Analyzing the impact of feature selection on heart disease prediction

With the spirit of reproducible research, this repository contains all the codes required to produce the results in the manuscript: 

> Pathan, M. S., Nag, A., Pathan, M. M., & Dev, S. (2022). Analyzing the impact of feature selection on the accuracy of heart disease prediction. Healthcare Analytics, 2, 100060.

All codes are written in `PYTHON`. The manuscript can be accessed from [this](https://arxiv.org/pdf/2206.03239.pdf) link.

Please cite the above paper if you intend to use whole/part of the code. This code is only for academic and research purposes.

### Code

+ `./Figures/corr_CVD.png`: The correlation values for each medical features of CVD dataset and the target feature stroke.
+ `./Figures/Corr_framingham.png`: The correlation values for each medical features of framingham dataset and the target feature TenYearCHD.
+ `./Figures/featscore_cvd.png`: The feature importance scores of each feature of CVD dataset for detecting stroke using the ANOVA-F test.
+ `./Figures/featscore_fram.png`: The feature importance scores of each feature of Framingham dataset for detecting TenYearCHD using the ANOVA-F test.
+ `./Dataset/`: This folder contains both our input datasets `CVD_Data.csv` and `framingham.csv`.

#### Scripts

+ `./Scripts/Stroke_paper.ipynb`: This code file contains all the code used for generating the results presented in the manuscript. In the manuscript we have presented results for two different datasets, however in the code file we have only included the code for framingham dataset as the procedure is same for both datasets. The code contains functions for data preprocessing such as class imbalance and null value problems. Furthermore, we have obtained the Correlation values using `.corr()` function of `Pandas` library in Python and have plotted the results using `seaborn` data visualisation library. The feature importance scores are generated using ANOVA-F statistical test. Finally, we used `Lazy Predict` library to build various basic ML models for the prediction task.  
