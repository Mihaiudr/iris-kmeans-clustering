## SPECIES SEGMENTATION WITH CLUSTER ANALYSIS (IRIS DATASET)

This project applies the K-Means clustering algorithm to the classic Iris flower dataset to perform unsupervised species segmentation.

The primary goal is to group the flowers into distinct clusters based only on their four physical measurements (sepal length, sepal width, petal length, petal width) and then evaluate how well these derived clusters correspond to the known species labels.

PROJECT FILES

Cluster Analysis.ipynb

The main Jupyter Notebook. It contains the complete workflow: data loading, feature scaling, determining the optimal number of clusters using the Elbow Method, K-Means implementation, and comparison of the clustering results against the true species labels.

iris_dataset.csv

The raw input data containing only the four features (sepal_length, sepal_width, petal_length, petal_width). This is the dataset used for the unsupervised clustering.

iris_with_answers.csv

The complete dataset, including the actual 'species' labels. This file is used in the final steps of the notebook for validation and performance evaluation.

clustering.yml

A Conda environment file listing all necessary Python packages and their specific versions required to run the project without dependency conflicts.

## SETUP AND INSTALLATION

This project requires a Python environment and the specified libraries. The recommended way to set up is using Conda with the provided environment file:

Step 1: Download or clone all project files.
Step 2: Navigate to the project directory in your terminal.

Step 3: Create the Conda environment:
conda env create -f clustering.yml

Step 4: Activate the new environment:
conda activate clustering

## HOW TO RUN THE ANALYSIS

Ensure the 'clustering' Conda environment is active.

Launch Jupyter Lab or Jupyter Notebook:
jupyter lab

Open the 'Cluster Analysis.ipynb' file.

Run all cells sequentially to execute the full data analysis, clustering, and visualization steps.

KEY DEPENDENCIES

The main libraries used for this analysis (defined in clustering.yml) are:

pandas / numpy: Data manipulation

scikit-learn: K-Means clustering model

matplotlib / seaborn: Data visualization (e.g., Elbow Plot, cluster scatter plots)

## END OF FILE
