# Final Project

### Project Topic: Predicting Housing Prices
### Project Author: Yuxi Zhang

## About this script
script filename: house_prices_predict_model.ipynb

dataset filename: boston_house_prices.csv

## The process of obtaining results
1. Downloading "Boston House Price" dataset from kaggle.com;
2. Using jupyter notebook to write the script file;
3. The version of the modules:
   - pandas: 1.4.2 
   - numpy: 1.21.5 
   - matplotlib: 3.5.1 
   - seaborn: 0.11.2 
   - sklearn: 1.0.2 
4. Using read_csv() from pandas to read the dataset;
5. Using matplotlib and seaborn to visualize the relationship between the data, use plt.savefig() to save images;
   - Linear relationship: dataset_scatter.png
   - Correlation relationship: dataset_heatmap.png
6. Import sklearn, using train_test_split() to divide dataset into training set and test set;
7. Training model，using r2_score() to obtain model score，save the visualization chart of predicted results and actual results，check the discrete degree predicted results;
   - prediction_scatter.png
8. Using joblib.dump() to save the training model，and joblib.load() to road local model;
   - BostonHousePriceLinearModel.skln
9. Final, using input() to enter the parameters and estimate the price of the house;