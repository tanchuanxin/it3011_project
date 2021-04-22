# it3011_project

Notebooks are found in the folders with two digits at the front. To run any of the notebooks, please pull them into the root directory to get access to necessary files and directory structure. Also mount the drive accordingly within the notebook.

You will need to clone the data yourself (6GB) and run the data processing notebook 00_create_dataset/00_create_dataset_no_na.ipynb to generate the dataset, if you wish to run any of our notebooks.

ACTIVE NOTEBOOKS
00_create_dataset - used to create our dataset, since the original data is too big for us to process on colab resources
01_exploration - used to inspect the data and draw some conclusions through visualization and statistical measures
04_tml_cv_baseline - notebooks using traditional machine learning, with cross validation
05_tml_cv_pca - notebooks using traditional machine learning and implementing PCA, with cross validation
06_tml_test - evaluating the best model obtained through cross validation among traditional machine learning models, on the actual test set
11_nndl_cv_mlp1 - notebooks using neural networks and deep learning, with cross validation
12_nndl_cv_mlp2 - notebooks using neural networks and deep learning, with cross validation (different model without dropout on input layer)
13_nndl_test - evaluating the best model obtained through cross validation among neural networks, on the actual test set

ACTIVE FOLDERS
data - contains the csv files with data
presentations - for presentations and report
results_nndl - folder with the figures and histories and model checkpoints for neural networks
scores - folder with the output scores from every model that we trained, both TML and NNDL

DEPRACATED - these were valid only for the interim presentation
02_tml_baseline_interim - notebooks using traditional machine learning
03_tml_pca_interim - notebooks using traditional machine learning and implementing PCA
archive - old code
