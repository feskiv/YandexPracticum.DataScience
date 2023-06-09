## Задача проекта
Необходимо построить модель машинного обучения классификации для рекомендации подходящего тарифа.

## Описание проекта
В распоряжении предобработанные данные о поведении клиентов, которые уже перешли на рассматриваемые тарифы. Для подбора подходящего тарифа нужно построить модель с максимально большим значением accuracy и довести долю правильных ответов по крайней мере до 0.75. 

## Стек
Pandas, Scikit-Learn

## Вывод
Для подбора наиболее подходящего тарифа на основе данных о поведении клиентов были обучены 3 модели: дерево решений, случайный лес и логистическая регрессия.

Наилучший результат показала модель случайного леса с accuracy = 0,80 и следующими гиперпараметрами:

max_depth = 8
n_estimators = 40
Модель дерева решений также достаточно точна (0,78). Наименьшая точность у логистической регрессии (0,71).

При проверке модели случайного леса на тестовой выборке точность снизилась совсем не существенно, а при сравнении с простейшей моделью DummyClassifier точность оказалась более, чем на 10% выше.

Исходя из оценки точности и проверки на адекватность наиболее подходящяя модель для решения задачи классификации - модель случайного леса.

## Статус
Проект завершен
