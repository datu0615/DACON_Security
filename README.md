# DACON_Security
![20220524_131028](https://user-images.githubusercontent.com/84311270/170263599-aed0ac9e-4e63-4e93-a5de-4854a2acea49.png)  
로그 데이터를 통해 시스템의 보안 위험도 등급을 예측   
기존에 없던 패턴의 공격 탐지  

## Dataset
1. train.csv  
id : 데이터 식별자  
level : 보안 위험 등급(0~6)  
full_log : 학습 데이터 전체 로그  


2. test.csv  
id : 데이터 식별자  
full_log : 테스트 데이터 전체 로그  
train.csv에 존재하지 않는 level 존재(0~7)  

3. sample_submission.csv  
id : 데이터 식별자  
level : 예측 level 작성  

4. validation_sample.csv  
full_log : 7등급 보안 로그 샘플  
학습 데이터로 활용 금지  
학습 완료후 추론과정 검증데이터로만 활용 가능  

## Model
Self Attention model을 사용하여 학습을 진행.

