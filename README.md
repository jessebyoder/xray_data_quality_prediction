This is the readme for the software pipeline "PDB Quality Predictor"
Authored by Jesse Yoder, June 2022

This pipeline creates a machine learning model based on the hardware used
in X-ray crystallography experiments

General instructions - 
1. All steps are organized in Notebooks, substeps are in functions
2. The bottom of each Jupyter notebook has the necessary functions
3. Jupyter notebooks are numbered in logical order

Intializing the database:
    Obtain the CSVs for initial download from the RCSB PDB web interface
        https://www.rcsb.org/search/advanced
    Search for "Structural Attribute" > "Experimental Method" > "X-RAY DIFFRACTION"
    Download the CSVs (multiple) with entry ID information
    Run "0_DataFrame_Initial_Assembly.py" notebook


Updating the database (not required immediatly after initialization):
    Run "1_DataFrame_Update_Pipeline.py" notebook
    
Cleaning the database:
    Run "2_DataFrame_Cleaning.py" notebook
    
Training the ML Model:
    Run "3_Data_Regression.py" notebook