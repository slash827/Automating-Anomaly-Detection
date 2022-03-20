# tds project

Our Anomaly Detection automation tool, used to help with the model-selection problem, and automating it.

## Installation

Because we use metaOD pre-trained model, we need to make sure we install this project on a **fresh** linux environment, because metaOD depends on specific version of scikit-learn (0.22.1)

## usage

After loading the datasets (there are for types of datasets attached, but can be done with more)
We run
```
X_train, y_train, X_test, y_test = load_data('pyod') #loading pyod data for example
best_model, results = automate_model_selection(X_train, y_train)
#then to plot it we run
plot_results_dict(best_model, results)
```

