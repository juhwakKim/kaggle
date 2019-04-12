kaggle or Datacon Guide
================
전체 과정
--------
1. 데이터 수집
2. 데이터 EDA
3. feature Engineering
4. model 결정
5. 평가


# 데이터 수집
https://dacon.io/index.php?mid=cpt6&category=65535&document_srl=62809 에서 다운로드 받는다
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import os
import numpy as np
```
필요한 라이브러리들을 import 한다.
```python
os.chdir("C:\\Users\\RND\\DaconDataset")
```
데이터를 다운로드받은 위치를 설정해준다.(윈도우에서는 \표시를 두번써준다)
```python
regular = pd.read_csv("Regular_Season_batter.csv")
```
```python
pd.set_option('display.max_columns', 500)
regular.head(10)
```
모든 column의 이름을 보기위해 Max값을 늘려준다

# 데이터 EDA
```python
regular.columns
```
어떤 카테고리(column)들이 있는지 확인한다.
```python
regular[['year','team','avg']]
```
위와 같이 쓰면 원하는 카테고리만 골라서 볼 수있다.
```python
regular['year'].describe()
```
특정 카테고리의 통계적 특징들을 볼수 있다.
```python
sns.distplot(regular['AB'])
```
그래프를 그려서 한눈에 볼 수 있다.



# feature Engineering




# model 결정




# 평가



