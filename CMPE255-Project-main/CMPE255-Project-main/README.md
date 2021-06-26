# CMPE255-Project
### Dataset Information
The dataset used for this project was BRFSS information from 2015. This dataset can be found at https://www.kaggle.com/cdc/behavioral-risk-factor-surveillance-system. The 2015 dataset has a size of 596 MB and is composed of 330 columns and 441,000 rows with approximately 80 million non-zeros values. Most of these values are categorical and represented by numbers; however, the meaning of such numbers can be looked up in a codebook provided by BRFSS that can be found at https://www.cdc.gov/brfss/annual_data/2015/pdf/codebook15_llcp.pdf

The Behavioral Risk Factor Surveillance System (BRFSS) is a public health survey conducted on approximately 400,000 people between the years of 2011 and 2015. BRFSS collects health information by conducting telephone surveys on U.S. residents from all 50 states. The information collected is related to risk behaviors, chronic health conditions, and preventable infectious diseases. Other factors considered are tobacco use, HIV/AIDS prevention, physical activity, and the consumption of fruits and vegetables.

The latest information offered by BRFSS is from the year 2015. In this project, the objective is to use the data from the latest year to predict the susceptibility of 4 different health issues: heart attack, diabetes, cancer, and depression based on other health information collected from various people.

![alt text](https://github.com/JanetteLopezUrzua/CMPE255-Project/blob/main/System%20Design.png?raw=true)


### Heart Attack Prediction
#### Prerequisites
* Install Anaconda from https://www.anaconda.com/products/individual. It should include Jupyter Notebook.
* Install XGBoost by going to Heart attack folder > CMPE255_Project_Preprocessing.ipynb, uncomment the first line that says "#!pip install xgboost" and run it.

#### To use the small test sample based from the preprocessed_dataset
* Go to the Heart attack folder > CMPE255_Project_Classification.ipynb and uncomment the line where it gets the data/test_sample dataset.
* Run the code to fit the models and check for recall on positive.

### Cancer Prediction
#### Prerequisites
  * Install Jupyter using [https://jupyter.org/installand](jupyter) Anaconda using [https://docs.anaconda.com/anaconda/install/](Anaconda)
  * Install XGBoost with the below command using Anaconda
    
    `conda install -c anaconda py-xgboost`
#### Open Notebook CMPE255_Project_Classifications.ipynb
  * Change the Read data cell from 'data/preprocessed_dataset.csv' or 'data/2015.csv' to 'data/small_size_dataset.csv' or 'data/preprocessed_dataset_test.csv'for training and testing the model for small dataset.
  * Train all the models and check for the recall scores for performance.
