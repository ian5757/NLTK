# NLTK

##  크리스마스 선물 추천

### 크리스마스 선물을 검색했을 때 등장하는 단어의 빈도
![output](https://user-images.githubusercontent.com/103472858/206586019-4f0e3115-068d-41cd-a1fa-3b1d97e6a7f0.png)

### to WordCloud
![wordcloud](https://user-images.githubusercontent.com/103472858/206586087-98b1bd0f-3125-40f1-bde1-ee4d2398a60b.png)

### 단어들의 상관관계 분석
```
data = word2vec.LineSentence(data_file)
model = word2vec.Word2Vec(data, vector_size=200, window=10, hs=1, min_count=2, sg=1)
```
> 사람들은 어떤 무드등을 좋아할까?
```
model.wv.most_similar(positive=['무드등'])
```
```
[('달', 0.8208963871002197),
 ('수면', 0.8048258423805237),
 ('아크릴', 0.802811324596405),
 ('nico', 0.7927249073982239),
 ('LED', 0.7919253706932068),
 ('조명', 0.7912560105323792),
 ('수유', 0.7867317795753479),
 ('램프', 0.7761112451553345),
 ('선풍기', 0.7591735124588013),
 ('취침', 0.7515832185745239)]
 ```
