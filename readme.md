# The Code of SIKT Model
This file is a tutorial for running SIKT model code.
## introduction
- model/
    - checkpoints/ :*Folder of model checkpoint*
    - log/  : *Folder of training log. There are log files of our paper.*
    - SIKT Model.ipynb : *SIKT model of Continual learning sequence train and joint train. *
- DataProcess/
    - raw_data/   : *Raw data of three dataset, ASSIST2009NSB=A09, ASSIST2012=A12, EdNet=EN*
    - test_data/  : *Test data of three dataset*
    - train_data/  :  *Train data of three dataset*
    - Data Process.ipynb : *Code of data process,if want to get the result in our paper, you need to run it.*
    - t-SNE.ipynb : *Code of t-SNE analysis*
- requirements.txt : *This file may be used to create an environment using:$ conda create --name <env> --file <this file>*
 

## setup
platform: linux-64

RAM: 120G

Please ensure that the version of Python is 3.8 and install all library files of requirements.txt.

You can use jupyter to run this code, or you can save it as a py file to run it.

## Run SIKT model
If you only want to run the model, you can directly enter *model/SIKT Model.ipynb*, run all the code to see that the model is training. Because the raw dataset is too large, only the first 50000 pieces of data are taken from each data set for demonstration.

## Run Data process
To restore the results of the article, enter *DataProcess/Data Process.ipynb* and run all the codes to generate all the data. It takes a long time to run this code and ensure that the computer has a large memory. Run *model/SIKT Model.ipynb* again, and you can reproduce the results in the article.

### t-SNE
If you have run Data Process.ipynb, you can run the t-SNE.ipynb, and see the data distribution of the three datasets.
    
