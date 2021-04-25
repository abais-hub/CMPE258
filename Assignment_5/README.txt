
Part A) End2End tfx pipeline with EDA, visualization on Chicago Taxi dataset
1. Added calculate distance travelled by cab, related histogram visuals
2. Added avg distance travelled
3. Added avg fare/mile
4. Histogram visuals for all fare paid
5. swarmplot of trip start vs fare
6. Hyper parameter tuning, experimented with changing the following
optimizer = 'rmsprop'
patience = 5
factor = 0.75
min_lr = 1e-10
metrics = rmse

Part B) End2End tfx interactivecontent pipeline on Chicago Taxi dataset
1. Examined apart from anamolies what other items could be inspected
2. Fixed code for ExampleGen train/split to get code to work
3. Added hyper parameter tuning
optimizer = 'rmsprop'
patience = 5
factor = 0.75
min_lr = 1e-10
metrics = rmse
4. Fixed model artificat dir to enable serving

Part C) Implement the solution using pytorch on Chicago Taxi dataset
1. Searched kaggle for NYC taxi fare prediction dataset. This is no longer available. Proof provided in colab.
2. Picked Chicago taxi dataset identical to Part A, Part B and redid part C on Chicago Taxi.
3. Added data ingestion stage for chicago taxi.
4. Added data pre-processing for chicago taxi.
5. Added train/test split for chicago taxi.
6. Added data prep for modelling.
7. Added hyper parameter tuning
8. Edited the fit API to work only on continous data, NYC taxi fare prediction has both categorical and continous data. Not so in chicago taxi.
9. Edited the pytorch dataloaders.
10. Edited the test API for chicago taxi.
11. Edited make predictions API to make predictions only on continous data.
 
Part D) Implement the solution using xgboost on Chicago Taxi dataset
1. Added data ingestion stage for chicago taxi.
2. Added data pre-processing for chicago taxi.
3. Added train/test split for chicago taxi.
4. Added data prep for modelling.
5. Added hyper parameter tuning
# train
gbm = lgb.train(params,
                lgb_train,
                num_boost_round=999,
                valid_sets=lgb_eval,
                early_stopping_rounds=20)
6. Edited K-fold cross validation to try 6 fold validation for improved QOR.
	
