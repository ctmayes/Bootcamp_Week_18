# Bootcamp_Week_18

# PyChain Ledger

This program is designed to build a blockchain-based ledger system, complete with a user-friendly web interface for a decentralized finance team. This ledger should allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.

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

At the beginning of the *pychain.py* file, the technologies are calling in with this code:

```
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
import datetime as datetime
import pandas as pd
import hashlib
```

---

## Usage

To operate this program, open up your terminal of choice and navigate to the directory in which you have downloaded the files within this repository. Run the relavant file with the command: 

```python
streamlit run pychain.py
```  

The Streamlit application will run locally in your browser and should launch automatically. From here you can enter the pertinent sender, receiver, and amount details to add to the ledger. This will be immediately updated and can be validated via the the ledger itself. 

---
## Validation Report

In the screenshot below we can clearly see a blockchain consisting of several entries, and functional and validated side-bar options, as well as a confirmation that the blockchain is valid.

!Ledger](./Resources/capture_ledger.png)


---

## Contributors

Colton Mayes ctmayes@gmail.com

---

## License

This code is created for educational purposes, and it usage therein has no commerical application. It is designated as free-use thusly, and shall remain as such.