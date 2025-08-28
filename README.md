  # 건설용 자갈 암석 종류 분류 AI 경진대회
### 알고리즘 | 월간 데이콘 | 비전 | 분류 | macro-f1
[236471-1-499929.pdf](https://github.com/user-attachments/files/22027351/236471-1-499929.pdf)

public, private 리더보드에서 최종 1위를 기록하였습니다.
* public score (1st) : 0.93557
* private score (1st) : 0.93563

## 1. 환경 설정
### 1-1. 저장소 코드 복사 
```
  git clone https://github.com/dd0nw/rock_classification_dacon.git
```
### 1-2. 패키지 설치
```
  conda env create -f environment.yaml
```
## 2. 폴더 구조
```
  ├── train
  │   ├── Andesite
  │   │   ├── TRAIN_00000.jpg
  │   │   ├── TRAIN_00001.jpg
  │   │   ├── TRAIN_00002.jpg
  │   ├── ...
  │   └── Etc
  │       └── TRAIN_xxxxx.jpg
  ├── test
  │   ├── TEST_00000.jpg
  │   ├── TEST_00001.jpg
  │   ├── ...
  │   └── TEST_xxxxx.jpg
  ├── sample_submission.csv
  ├── train.csv
  ├── test.csv
  └──Dacon_Final.ipynb
```


## 3. 모델 가중치

[tf_efficientnetv2_m.in21k_ft_in1k](https://docs.google.com/uc?export=download&id=1UBzks6KyGvaFzE2x5UzZ3boZsSygrcdn)
<br>
[tf_efficientnetv2_s.in21k_ft_in1k](https://docs.google.com/uc?export=download&id=1ozHgS0x4UlPHX0XIOYX5K3plOfq46tgK)
<br>
[regnety_120.sw_in12k_ft_in1k](https://docs.google.com/uc?export=download&id=1DvCZ0o1g9WkGlP2UinOR3_DD496tX-O1)
<br>
[tiny_vit_21m_384.dist_in22k_ft_in1k](https://docs.google.com/uc?export=download&id=1N7q-qQw2SQKxv6eXpLTONEPwaACrqaCL)

## 4. 개발환경
```
  OS :  Ubuntu 24.04.1 LTS
  GPU : RTX A6000(48GB), RTX 5080(16GB)
  CPU : Thread Threadripper 1950X, i5-14600k
  RAM : 64GB, 32GB
```

## 5. 데이터셋
[Dacon](https://drive.google.com/file/d/1UowP6kVAFXk1wkjTTD0hd3XOPgPKA0vp/view)
