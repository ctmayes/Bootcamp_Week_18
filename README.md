# Bootcamp_Week_18

# PyChain Ledger

This program is designed to improve the existing algorithmic trading systems at our firm and maintain the firm’s competitive advantage in the market. To do so, we are attempting to enhance enhance the existing trading signals with machine learning algorithms that can adapt to new data. Additionally, we compare a series of inputs that would drive these disparate results.

## Technologies

Within this program, we will make use of the following external python modules:

  -- pandas
  -- pathlib
  -- numpy
  -- sklearn
  -- matplotlib
  -- hvplot
  
  Additionally, this program was created within a python v3.7 build, and its relevant dependencies.

---

## Installation Guide

To utilize this program, within your terminal you will have to install the required libraries. Within your terminal, input the following commands:

```python
pip install pandas
```

```python
pip install pathlib
```

```python
pip install numpy
```

```python
pip install -U scikit-learn
```

```python
pip install matplotlib
```

```python
pip install hvplot
```

At the beginning of the *venture_funding_with_deep_learning.ipynb* file, the technologies are calling in with this code:

```
import pandas as pd
import numpy as np
from pathlib import Path
import hvplot.pandas
import matplotlib.pyplot as plt
from sklearn import svm
from sklearn.preprocessing import StandardScaler
from pandas.tseries.offsets import DateOffset
from sklearn.metrics import classification_report
```

---

## Usage

To operate this program, open up your terminal of choice and navigate to the directory in which you have downloaded the files within this repository. Open Jupyter Lab with the command: 

```python
jupyter lab
```  

This should open jupyter lab to the filepath in which you have the repo file, and you simply need double click the *venture_funding_with_deep_learning.ipynb* file to open it. Upon opening, select the menu button with two right facing arrows at the top of the notebook, which will run the entire file. It will ask you to confirm you wish to restart the file, to which you will confirm. Wait a few moments for the program to operate as intended, and peruse the resulting data at your leisure. If you wish, simply skip to the end for my analysis of the preceding information. 

---
## Evaluation Report

Baseline:

![Baseline_Comp](/Resources/Baseline.png)

Referencing the above graphic, the baseline model already outpaces actual returns, and therefore we have a fantastic stepping off point to continue to refine our model.

Tuning the training algorithm:

![Baseline_Comp](/Resources/ten_months.png)

What impact resulted from increasing or decreasing the training window?

Increasing the training window from 3 month to 10 months had an extremely detrimental effect on our strategy comapred with actual results, and was not a value add. It was still informative however.

![Baseline_Comp](/Resources/increased_windows.png)

What impact resulted from increasing or decreasing the training window?

By increasing our windows from 4/100 to 25/200, we are able to effectively(over enough time) mimic the actual returns with our modeled strategy. 

Choose the set of parameters that best improved the trading algorithm returns:

![New_Model_Comp](/Resources/combined.png)

In an interesting evolution, combining the two prior discussed modifications collectively outputs a highly effective strategy that outpaces actual returns in a meaninful way.

Evaluate a New Machine Learning Classifier:

![New_Model_Comp](/Resources/new_machine_model.png)

Did this new model perform better or worse than the provided baseline model? 

This new model performed much better initially, but over time its efficacy falls apart and is rendered as a negative addition to our modeling toolkit.


Did this new model perform better or worse than your tuned trading algorithm?

Our tuned algorithim was a clear upgade over the baseline model, and this new model is much worse than either sadly.

---

## Contributors

Colton Mayes ctmayes@gmail.com

---

## License

This code is created for educational purposes, and it usage therein has no commerical application. It is designated as free-use thusly, and shall remain as such.