<p align="center">
  <img src="https://github.com/Bae-hong-seob/NLP_project/assets/49437396/232c7e24-c7c2-4a24-918b-b31db569dcc6">
</p>

# How to Start?
[Download yelp dataset](https://www.yelp.com/dataset/download)
**Steps 1-4 must be run for each dataset.**

# 1. Make Total Datset
- run 'preprocess_file(make_splited_datasets).ipynb'
- make 7 splited datsets(if splited dataset have above 30,000 rows, do sampling(30,000)) 

# 2. Make Summary about 'text' column
- run 'make_summary.ipynb'
- cuz, sentiment analysis model has max length about input sequence

# 3. Make Sentiment score about 'summary' column
- run 'make_sentiment_score.ipynb'
- based on our Positive/Negative Scale Conversion Algorithm

# 4. Make ensemble model
- run 'make_ensemble.ipynb'
- Finally, we make final dataset that convert 'text' column to 'sentiment_score'
- Thus, input vector was created for the ML model.
- Ensemble model generation for 7 datasets

# 5. Use created Model
- run 'pycaret_model_load_and_prediction'
- After make ensemble model, you can load model and use.
