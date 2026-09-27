# Auto Loan Pricing Optimization

Python notebook for HADM 5285 Introduction to Machine Learning in Business (Cornell University, Spring 2026) that models whether customers accept auto loan offers and uses the model to choose revenue-maximizing interest rates (Nomis Solutions case).

Code:
- code/Mini_Project_2_Final_Version.ipynb : main notebook. Selects one customer segment (60-month used-car loans under $25,000, FICO strictly between 680 and 720), trims rate outliers, fits a logistic regression of acceptance on rate, and searches for the single rate that maximizes expected revenue. Then compares SVM, decision tree, random forest and neural network models on FICO, amount, competitor rate, rate, cost of funds and partner bin, picks the best by validation AUC, finds the optimal rate for each test customer, and explores feature importance and k-means clusters.

Data:
- data/ : the notebook reads CU262-XLS-ENG.xlsx (sheet "e_Car_Data_for_Case"), the data file for the Darden case "Nomis Solutions". It is copyrighted course material and is not included; put your copy in the same folder as the notebook.

Output:
- output/ : the figures produced by the notebook (saved from its cell outputs)

To run: open the notebook in Jupyter or Colab with pandas, numpy, matplotlib, seaborn, scikit-learn and tensorflow installed.
