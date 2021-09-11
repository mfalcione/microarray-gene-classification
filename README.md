# Gene Selection and Classification of Microarray Data using Various Machine Learning Techniques
In bioinformatics studies, the selection of relevant genes for sample classification is a common task.

The goal of this project is to compare the accuracy of the results obtained to those of the paper using various machine learning methods such as random forest, XGBoost, neural network, linear discriminant analysis (LDA), k nearest neighbor (KNN), logistic regression, and support vector machine (SVM). An additional goal is to investigate the performance of feature selection with algorithms used in the [reference paper](http://www.biomedcentral.com/1471-2105/7/3/abstract).

The reference paper obtained 10 cancer datasets from various sources. The colon, prostate, lymphoma, SRBCT, and brain datasets were obtained from Dettling and Buhlmann (2002). The leukemia dataset was filtered from Golub et al (2002). The adenocarcinoma dataset was taken from Ramaswamy et al (2003). The breast cancer dataset was taken from vant Veer et al (2002). Finally, the NCI 60 dataset was taken from Ross et al (2000).

Tree-based and Logistic Regression recursive feature elimination methods performed best with percent errors of 17.514% +/- 12.51% and 15.623% +/- 15.517%, respectively. Feature selection performance increases across all datasets for SVM ranged from 0% to 28.6% with an average of 8.47% +/- 8.73%, and performance increases across all datasets for KNN ranged from 0% to 14.3% with an average of 6.88% +/- 5.82%. The team’s models were able to produce better performance than those from the original paper for each dataset. The experiments also show that feature selection with SVM and KNN models produced a lower error rate than when they were run with the raw features. Logistic regression outperformed all other methods on average, but the random forest model performed best most consistently,

### Project Files
- **project.ipynb:** this is the data processing and results notebook. 
- **requirements.txt:** contains all the required python packages to streamline installation.
- **accuracy_list_final_output.pickle:** - final accuracy output from classification models (can be loaded into code to skip proprocessing and model classification)
- **auc_roc_list_final_output.pickle:** - final AUC-ROC output from classification models (can be loaded into code to skip proprocessing and model classification)

### Install Project Dependecies
The project is dependent on the following python packages:

```
scikit-learn==0.24.1
xgboost==0.90
numpy==1.20.0
requests==2.25.1
pandas==1.2.1
```

Alternatively one can install all the required packages by running the pip command below.

* `pip install -r requirements.txt`

### Runing the Code

- Refer to [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) or [Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/index.html#) documentation for instructions on running the code and setting up the notebook.
