# Machine Learning Foundations

A progression of implementation notebooks and mathematical work covering supervised learning, model evaluation, natural-language classification, and unsupervised representation learning.

## What I learned

- Performing exploratory data analysis, preprocessing mixed feature types, and reasoning about correlation and feature engineering
- Deriving and implementing linear regression with the normal equation and batch gradient descent
- Comparing learning rates, convergence behavior, validation error, and the effects of correlated features
- Implementing logistic regression with L1 and L2 regularization and measuring robustness to noisy data
- Applying perceptrons, kernel methods, and support vector machines to classification problems
- Building text classifiers with TF-IDF, linear and RBF kernels, and multinomial Naive Bayes
- Evaluating models with hyperparameter searches, accuracy curves, support-vector counts, and error analysis
- Exploring GloVe word embeddings with K-means clustering, PCA, and t-SNE
- Working through the linear algebra, probability, maximum-likelihood, maximum-a-posteriori, and Bayesian foundations behind the implementations

## Repository map

| Path | Focus |
| --- | --- |
| `notebooks/00-housing-data-exploration.ipynb` | Exploratory analysis and categorical preprocessing for housing data |
| `notebooks/01-linear-regression.ipynb` | Closed-form regression, gradient descent, normalization, and feature analysis |
| `notebooks/02-regularized-logistic-regression.ipynb` | Binary classification with L1/L2 penalties and noisy-data experiments |
| `notebooks/03-text-classification.ipynb` | TF-IDF features, SVM kernels, and multinomial Naive Bayes |
| `notebooks/04-embeddings-and-clustering.ipynb` | GloVe embeddings, K-means, PCA, t-SNE, and embedding-based classification |
| `data/` | Housing training and validation data used by the linear-regression notebook |
| `reports/implementation/` | Rendered outputs for the five implementation notebooks |
| `reports/written/` | Mathematical derivations and written model-analysis work |

## Running the notebooks

The notebooks preserve their original Google Colab cells and recorded outputs. For a local Jupyter environment:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
jupyter lab
```

The linear-regression CSV files are included in `data/`. The other notebooks reference course-provided files that are not available in this repository: `ia0_train.csv`, `IA2-train.csv`, `IA2-dev.csv`, `IA2-train-noisy.csv`, `IA3-train.csv`, `IA3-dev.csv`, and `GloVe_Embedder_data.txt`. To reproduce those notebooks, provide the files at the paths defined near the top of each notebook or update those path variables for the local environment.

The legacy PDF-export cells also expect `wkhtmltopdf`; the completed PDF reports are already available under `reports/`.
