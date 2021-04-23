# it3011_project

Jane Street Market Prediction - https://www.kaggle.com/c/jane-street-market-prediction

This is the README file for A0228402N-A0230521Y-A0230632U submission.
We are contactable through the following:

- A0228402N at e0673235@u.nus.edu
- A0230521Y at e0697782@u.nus.edu
- A0230632U at e0698539@u.nus.edu

# Running the notebooks

Notebooks are found in the folders with two digits at the front. To run any of the notebooks, please pull them into the root directory to get access to necessary files and directory structure. Also mount the drive accordingly within the notebook.

### Mounting drive

In the second code block of every notebook, you will see the following:

    ''' used to reference the root directory, for directory traversal '''
    from google.colab import drive
    drive.mount('/content/gdrive', force_remount=True)
    mount_dir = '/content/gdrive'
    root_dir = Path('/content/gdrive/My Drive/it3011_project')

Please amend the `root_dir` path to your google drive path, if different.

### Cloning data

You will need to clone the data yourself (6GB) from the competition website, and save it in the following directory

    |-- it3011_project
        |-- data
            |-- jane-street-market-prediction.zip (original data)
            |-- jane-street-market-prediction (unzipped version)
        |-- 00_create_dataset
            |-- 00_create_dataset.ipynb
            |-- 00_create_dataset_no_na.ipynb
        |-- ...

### Generating train/test set

Pull out the data processing notebook 00_create_dataset/00_create_dataset_no_na.ipynb into the root directory (it3011_project) and run it to generate the truncated dataset, if you wish to run any of our notebooks. The directory will look like this

    |-- it3011_project
        |-- data
            |-- jane-street-market-prediction.zip (original data)
            |-- jane-street-market-prediction (unzipped version)
            |-- test_no_na.csv (test set)
            |-- train_no_na.csv (train set)
        |-- 00_create_dataset
            |-- 00_create_dataset.ipynb
        |-- 00_create_dataset_no_na.ipynb (pulled out to root from the 00 folder)
        |-- ...

### ACTIVE NOTEBOOK FOLDERS

After generating the dataset, you can pull notebooks from any of the active notebook folders and run them in the root. Be sure to mount the drive accordingly

    00_create_dataset - used to create our dataset, since the original data is too big for us to process on colab resources
    01_exploration - used to inspect the data and draw some conclusions through visualization and statistical measures
    04_tml_cv_baseline - notebooks using traditional machine learning, with cross validation
    05_tml_cv_pca - notebooks using traditional machine learning and implementing PCA, with cross validation
    06_tml_test - evaluating the best model obtained through cross validation among traditional machine learning models, on the actual test set
    11_nndl_cv_mlp1 - notebooks using neural networks and deep learning, with cross validation
    12_nndl_cv_mlp2 - notebooks using neural networks and deep learning, with cross validation (different model without dropout on input layer)
    13_nndl_test - evaluating the best model obtained through cross validation among neural networks, on the actual test set

### ACTIVE DATA FOLDERS

These folders contains the outputs that we have created, in terms of model results

    data - contains the csv files with data
    presentations - for presentations and report
    results_nndl - folder with the figures and histories and model checkpoints for neural networks
    scores - folder with the output scores from every model that we trained, both TML and NNDL

### DEPRACATED - these were valid only for the interim presentation

    02_tml_baseline_interim - notebooks using traditional machine learning
    03_tml_pca_interim - notebooks using traditional machine learning and implementing PCA
    archive - old code
