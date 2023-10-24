# Краткое описание проекта
Необходимо обучить модель классифицировать комментарии на позитивные и негативные.

В вашем распоряжении набор данных с разметкой о токсичности правок.
Постройте модель со значением метрики качества F1 не меньше 0.75.

## Используемые инструменты
Библиотеки:
- matplotlib
- nltk
- numpy
- pandas
- sklearn
- spacy
- transformers
- torch
- wordcloud

Модели:
- SGDClassifier (sklearn.linear_model)
- LogisticRegression (sklearn.linear_model)
- RidgeClassifier (sklearn.linear_model)
- Perceptron (sklearn.linear_model)
- PassiveAggressiveClassifier (sklearn.linear_model)
- NearestCentroid (sklearn.neighbors)

Пайплайн:
- GridSearchCV (sklearn.model_selection)
- ColumnTransformer (sklearn.compose)
- StandardScaler, OneHotEncoder (sklearn.preprocessing)


## Вывод
Текст очищен от мусорных символов, лемматизирован средствами библиотеки Spacy.
С помощью Tfidf выделены признаки для обучения моделей.
Рассмотренны несколлько моделей для обучении.
Лучший результат показал LinearSVC() с результатом метрики f1 на тесте - 0.789
