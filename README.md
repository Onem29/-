Проект "Отток клиентов"

Описание проекта.
Из «Бета-Банка» каждый месяц стали уходить клиенты. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

Задача:
На основе предоставлены исторические данные о поведении клиентов и расторжении договоров с банком нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. 

Требования:
Постройте модель с предельно большим значением F1-score не менее 0.59.
Дополнительно измеряйте показатель AUC-ROC и сравнивайте его с значение F1-score.

Источник данных: https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling

Признаки:

* RowNumber — индекс строки в данных;
* CustomerId — уникальный идентификатор клиента;
* Surname — фамилия;
* CreditScore — кредитный рейтинг;
* Geography — страна проживания;
* Gender — пол;
* Age — возраст;
* Tenure — сколько лет человек является клиентом банка;
* Balance — баланс на счёте;
* NumOfProducts — количество продуктов банка, используемых клиентом;
* HasCrCard — наличие кредитной карты;
* IsActiveMember — активность клиента;
* EstimatedSalary — предполагаемая зарплата.

Целевой признак:
* Exited — факт ухода клиента.

В данном проекте для предсказания значения целевого признака использовались модели классического обучения, а именно: "Логистическая регрессия", "Случайный лес" и "SMV". Для решения проблемы несбалансированных значений признаков рассматривались методы "Upsempling" и "Downsempling", а также использование моделей с параметром balance.

В результате исследования выбрана модель "Случайный лес" с итоговой метрикой качества F1-score равной 0.606, что удовлетворяет требованиям проекта.