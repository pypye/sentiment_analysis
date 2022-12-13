# Sentiment Analysis Run and Submit Tutorial
*Sentiment Analysis by INT3405E_41_DMT (Duc Tran Van, Minh Tan Nguyen, Trung Hoang Nguyen)*
- Firstly, download [data.zip](https://github.com/pypye/sentiment_analysis/blob/main/data.zip) file above then extract and then open [int3405-phobert-vgg11.ipynb](https://github.com/pypye/sentiment_analysis/blob/main/int3405-phobert-vgg11.ipynb) config the cell like this, {BASE_DIR} is your current dataset directory you have extracted.
```py
DATASET_TRAIN_TEXT_FILE = '{BASE_DIR}/machine-learning-preproc/train_merged_segmented_v2.csv'
DATASET_TRAIN_IMAGE_FOLDER = '{BASE_DIR}/int3405-ml-preprocess-image-data-v2/image_train_resized'
DATASET_TEST_TEXT_FILE = '{BASE_DIR}/machine-learning-preproc/test_labelled_segmented.csv'
DATASET_TEST_IMAGE_FOLDER = '{BASE_DIR}/int3405-ml-preprocess-image-data-v2/image_test_resized'
```
- Secondly, install python library file in [requirements.txt](https://github.com/pypye/sentiment_analysis/blob/main/requirements.txt) if run in local, otherwise Colab or Kaggle, just skip this step.
- Thirdly, make sure **internet is connected** for model downloading and **GPU is activated** for model training.
- Fourthly, run all the cell in [int3405-phobert-vgg11.ipynb](https://github.com/pypye/sentiment_analysis/blob/main/int3405-phobert-vgg11.ipynb) and wait for training.
- Finally, we use **submission.csv** file to submit to [INT3405 - Sentiment Analysis Problem](https://www.kaggle.com/competitions/int3405-sentiment-analysis-problem)
```py
review_d.to_csv("submission.csv", index=False)
```
