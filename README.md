Chapter 17 activity:

- In this chapter we examined a dataset and used 4 different models to determine the accuracy score and speed for each off the models
- Models examined in this activity includes: kNN, Decision Trees, Logistic Regression, and SVM
- The datset was downloaded as part of the project, along with a PDF file, which clearly describes the collection method for the data
- As part of this reearch, the authors have also utilized a different approach which seems to be common for this kind of researches ( LIFT Curve )
- LIFT Curve is not covered as part of this exercise.


Gven the size of the data, I chose to run my notebook in google colab, so this notebook, in addition to this repositry, it is available in colab.


Structure:
README.md
Dataset: data/bank-additional-full.csv
notebook: prompt_III-Amin.ipynb


Process:

- There are 20 features available in dataset.
- There is one target column "y", which represents whether or not the client was subscribed.

As part of this exercise, we will use the first 7 features + target column.

The process, code and explaination has been included in each section and there should be comments in the code.

1 - A base model and score was established using default.
2 - Then we did a comparison of the score and time it took for the 4 models and created its own result_df.
3 - Then we added additional hyper parameters to continue comparing the 4 models in regards with score and execution time.
4 - I provided, Model,Best Parameters,Train Time,Train Accuracy,Test Accuracy and ROC-AUC Score in result_df
4 - At the end I also took decision tree using the best suggested parameter and provided an overview of decision tree.


Observations:
- The feature importance between logistic regression and decision tree are different. which highlights the importance of selecting the right model
- SVM took roughly executed 100 times slower than other 3 models with default values and when attempted to use hyper parameters after waiting 40 mins, it never completed. I noted some of the issues why SVM might have not been a good fit, but at this point I cannot be certain.
