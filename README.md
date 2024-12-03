# Updated multi-layer perceptron algorithm for predicting solute transport parameters and processes in karst conduits with variable flow rates
#### **MLP models for prediction of breakthrough curves in karst conduits with variable flow rates**  
This repository contains Python code for the MLP model. MLP is composed of two major components: the training process including optimization of hyperparameters, and then the prediction of the breakthrough curves in karst conduits with variables flow rates.
We rely on Python 3.6, along with the libraries Numpy, Pandas, scikit-learn, Matplotlib, alongside TensorFlow and Keras for deep-learning implementation.
The original datasets used in this repository have been retrieved from the reference below. 
Reference:Zhao X, Chang Y, Wu J, Xue, X., 2019. Effects of flow rate variation on solute transport in a karst conduit with a pool. Environ. Earth Sci. 78, 237. https://doi.org/0.1007/s12665-019-8243-y.
Note that the code is in Jupyter Notebook format and requires modification to use with other datasets.
#### **OTIS programs for simulation of breakthrough curves to obtain the transport parameters**  
This repository also contains OTIS programs for simulation of the predicted breakthrough curves, and the user's guide of OTIS. 
Reference:Runkel, R.L., 1998. One-dimensional transport with inflow and storage (OTIS): A solute transport model for streams and rivers. US Department of the Interior, US Geological Survey. https://doi.org/10.2307/1293197.

  
## Installation guide
#### **Python and packages**  
Download Anaconda3-2021.05-Windows-x86_64.exe on https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/
#### Installing different compilation environments:
conda create -n py36 python=3.6
activate py36
#### **Tensorflow and Keras installation:**  
pip install tensorflow - gpu == 2.0.0 / 2.1.0
pip install keras == 2.3.1
#### **Pands, Matplotlib and Jupyter Notebook installation**     
pip install pandas
pip install matplotlib
pip install jupyter
conda install nb-conda
#### **Installing the program of Bayesian optimization**     
pip install -i https://pypi.douban.com/simple bayesian-optimization

Libraries used:
 - tensorflow
 - keras
 - pandas
 - numpy
 - scipy
 - matplotlib
 - jupyter  
 - scikit-learn

## Content
* **Original Data in 'MLP_Jupyter Notebooks':** original data in three scenarios: BTCdata_b1-9 and BTCdata_c1-9 indicate the inpute variables and output concentration data of MLP in S1, BTCdata_b+c indicates the inpute variables and output concentration data of MLP in S2, and BTCdata_a+b+c indicates the inpute variables and output concentration data of MLP in S3
* **MLP_Jupyter Notebooks:** the python codes of MLP models edited in Jupyter notebook, they can be run to predict the breakthrough curves in conduits with different flow rates  
In the file names, 'b'or'c'means scenario S1, 'bc'means scenario S2, and 'abc'means scenario S3;'b1-b9' or 'c1-c9' means test data in the three scenarios.
* **OTIS:** OTIS programs, they can be run to estimate the solute transport parameters by simulating the predicted breakthrough curves. Then, we obtain the predicted solute transport parameters. 

