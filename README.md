# Fake or Real : AI 생성 이미지 판별 경진대회

## Code setting (Final)

### 1. train_config.yaml

* DIRECTORY: 
  dataset: #{DATA_DIR}/train
  
  * #{DATA_DIR} → /content/baseline

* learning_rate : 4.0e-4
* n_epochs : 2
* batch_size : 25(32)


### 2. predict_config.yaml

* DIRECTORY:
  dataset: #{DATA_DIR}/test/images
  sample_submission_path : #{DATA_DIR}/test/sample_submission.csv
  
  * #{DATA_DIR} → /content/baseline

* TRAIN:
  train_serial: #'YYYYMMDD_HHMMSS'
  
  * After training, you might get it from 'result' directory
  * #'YYYYMMDD_HHMMSS' → (ex) '20230705_150000'
