# Imbaqu
This package called "imbami" (Imbalance Mitigation) implements the methods for the mitigation of data imbalance as described in the corresponding article "Model-agnostic Mitigation Strategies of Data Imbalance for Regression". The article is available [here add link](www.offis.de).

The goal of imbami is to provide the scientific community with a set of relevance functions and mitigation methods to tackle problem of data imbalance. The following relevance functions and mitigation methods are included: 
* Relevance Functions
  * **Density-distance relevance**
  * **Density-ratio relevance**
* Mitigation Methods
  * **continuous SMOGN (cSMOGN)**
  * **continuous ratio-based SMOGN (crbSMOGN)**



If used, please cite:
```
@article{imbami,
  author       = {Wibbeke, Jelke and Rohjans, Sebastian and Rauh, Andreas},
  title        = {Model-agnostic Mitigation Strategies of Data Imbalance for Regression},
  year         = {XXX},
  publisher    = {}
}
```

## Requirements and Installation
Download the package from GitHub, navigate to the `setup.py` and install it using pip:
```
pip install .
```
The package was tested using:
```
python=3.10.13
numpy=1.26.4
pandas=2.1.4
KDEpy=1.1.11
```

Other versions may also work, but have not been tested.

## Usage
# ToDo!
```python
# mIR continuous
mir = imbaqu.mean_imbalance_ratio(data['num1'])
print(f'mIR of a continuous variable: {mir:.2f}')

# mIR discrete
mir = imbaqu.mean_imbalance_ratio(data['cat1'], discrete=True)
print(f'mIR of a discrete variable: {mir:.2f}')
```
For further explanation see the [example notebook](example.ipynb).
