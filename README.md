[![Build](https://github.com/gabalz/dcfit/actions/workflows/python-package.yml/badge.svg)](https://github.com/gabalz/dcfit/actions/workflows/python-package.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# DCFit package

A Python library of delta-convex fitting algorithms.

-------------------------------------------------------------------------------------------------
## References

> Near-optimal delta-convex estimation of Lipschitz functions, \
> *Gabor Balazs,* \
> arXiv, 2025 ([paper](https://doi.org/10.48550/arXiv.2511.15615)).

--------------------------------------------------------------------------------------------------
## PYTHON ENVIRONMENT

The installation of a minimal virtual environment to show the requirements of running the code.

```bash
python3 -m venv .../pyenv  # creating empty virtual environment
source .../pyenv/bin/activate  # activating the virtual environment

pip install --upgrade pip
pip install --upgrade setuptools

cd .../cvxreg
pip install -r requirements.txt  # recommended
# or
# for the latest package versions:
# pip install numpy scipy osqp clarabel numba
# pip install scikit-learn scikit-fda xgboost  # for running the notebook

# Jupyter notebook (optional):
pip install joblib pandas widgetsnbextension jupyter matplotlib seaborn papermill
```

-------------------------------------------------------------------------------------------------
## EXPERIMENTS

For examples, explore the `dataset.ipynb` notebook which can run experiments on various public datasets.

-------------------------------------------------------------------------------------------------
## UNIT TESTING

All the tests can be run by using pytest:
```bash
source .../pyenv/bin/activate  # if not done yet
pip install pytest seaborn
cd .../dcfit  # go to the root directory of this project
PYTHONPATH=. pytest dcfit/test/
```
