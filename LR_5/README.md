# Лабораторная работа №6: Машины опорных векторов
## Вариант 5
## Задание.
- Данные своего варианта из упражнения 3 (на регуляризацию и снижение размерности)
разделить на выборку для построения моделей (85%) и отложенные наблюдения (15%).
Отложенные наблюдения использовать только для прогноза по лучшей модели.
- Построить два пайплайна моделей, каждый из которых включает преобразование
объясняющих переменных (например: шкалирование, PCA, PLS) и модель классификации
(например: LDA, QDA, логит, случайный лес, svm - обязательно). Провести настройку
параметров каждой модели, которая содержит настроечные параметры, с помощью
сеточного поиска.
- Довести точность лучшего пайплайна (на обучающих данных, с перекрёстной
проверкой) до 96% и выше.
- Сделать прогноз по лучшей модели на отложенные наблюдения и оценить его точность.
## Выполнение.
1. Считан файл с данными, определены константы, удалены лишние переменные. Получины выборки: тестовая, тренировочная.
2. Предварительный анализ данных показал, что все переменные имеют числовое значение,Пустые значе ния отсутствуют.
3. Построены модели: модель с использованием StandartScaler() и SVC(); модель с использованием StandartScaler() и RandomForestClassifier().
4. Точность 1 модели по Acc = 0.798, точность 2 модели по Acc = 0.827.
5. Сделан прогноз по vjltkb 2 на отложенных наблюдениях, точность получилась 0.85.
