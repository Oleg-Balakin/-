# Финальный прект Яндекс Практикум

# Телеком — прогноз оттока клиентов
Оператор связи «Ниединогоразрыва.ком» хочет научиться прогнозировать отток клиентов. Если выяснится, что пользователь планирует уйти, ему будут предложены промокоды и специальные условия. Команда оператора собрала персональные данные о некоторых клиентах, информацию об их тарифах и договорах.

# Задача
Построить прототип модели машинного обучения. 

# Описание услуг
Оператор предоставляет два основных типа услуг:

Стационарную телефонную связь. Возможно подключение телефонного аппарата к нескольким линиям одновременно.
Интернет. Подключение может быть двух типов: через телефонную линию (DSL, от англ. digital subscriber line, «цифровая абонентская линия») или оптоволоконный кабель (Fiber optic).
Также доступны такие услуги:

Интернет-безопасность: антивирус (DeviceProtection) и блокировка небезопасных сайтов (OnlineSecurity);
Выделенная линия технической поддержки (TechSupport);
Облачное хранилище файлов для резервного копирования данных (OnlineBackup);
Стриминговое телевидение (StreamingTV) и каталог фильмов (StreamingMovies).
За услуги клиенты могут платить каждый месяц или заключить договор на 1–2 года. Доступны различные способы расчёта и возможность получения электронного чека.

# Описание данных
Данные состоят из файлов, полученных из разных источников:

contract.csv — информация о договоре;
personal.csv — персональные данные клиента;
internet.csv — информация об интернет-услугах;
phone.csv — информация об услугах телефонии.
Во всех файлах столбец customerID содержит код клиента.

Информация о договорах актуальна на 1 февраля 2020.

# Описание полей данных
BeginDate - дата начала пользования услугами;
EndDate - дата окончания пользования услугами;
Type - тип оплаты: ежемесячный, годовой и т.д.;
PaperlessBilling - электронный платежный документ;
PaymentMethod - способ оплаты;
MonthlyCharges - ежемесячные траты на услуги;
TotalCharges - всего потрачено денег на услуги;
Dependents - наличие иждевенцев;
Senior Citizen - наличие пенсионного статуса по возрасту;
Partner - наличие супруга(и);
MultipleLines - наличе возможности ведения параллельных линий во время звонка.

# Требования качества
Метрика AUC-ROC > 0.85
