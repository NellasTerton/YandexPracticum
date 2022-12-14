Вы аналитик компании «Мегалайн» — федерального оператора сотовой связи. Клиентам предлагают два тарифных плана: «Смарт» и «Ультра». Чтобы скорректировать рекламный бюджет, коммерческий департамент хочет понять, какой тариф приносит больше денег.
Вам предстоит сделать предварительный анализ тарифов на небольшой выборке клиентов. В вашем распоряжении данные 500 пользователей «Мегалайна»: кто они, откуда, каким тарифом пользуются, сколько звонков и сообщений каждый отправил за 2018 год. Нужно проанализировать поведение клиентов и сделать вывод — какой тариф лучше.

<b>Описание тарифов</b> 
<br>Тариф «Смарт»
<br>Ежемесячная плата: 550 рублей
<br>Включено 500 минут разговора, 50 сообщений и 15 Гб интернет-трафика
<br>Стоимость услуг сверх тарифного пакета:
<br>минута разговора: 3 рубля
<br>сообщение: 3 рубля
<br>1 Гб интернет-трафика: 200 рублей

<b>Тариф «Ультра»</b> 
<br>Ежемесячная плата: 1950 рублей
<br>Включено 3000 минут разговора, 1000 сообщений и 30 Гб интернет-трафика
<br>Стоимость услуг сверх тарифного пакета:
<br>минута разговора: 1 рубль
<br>сообщение: 1 рубль
<br>1 Гб интернет-трафика: 150 рублей
# Описание данных
<b>Таблица users (информация о пользователях):в</b>
<br>user_id — уникальный идентификатор пользователя
<br>first_name — имя пользователя
<br>last_name — фамилия пользователя
<br>age — возраст пользователя (годы)
<br>reg_date — дата подключения тарифа (день, месяц, год)
<br>churn_date — дата прекращения пользования тарифом (если значение пропущено, то тариф ещё действовал на момент выгрузки данных)
<br>city — город проживания пользователя
<br>tariff — название тарифного плана

<b>Таблица calls (информация о звонках):</b>
<br>id — уникальный номер звонка
<br>call_date — дата звонка
<br>duration — длительность звонка в минутах
<br>user_id — идентификатор пользователя, сделавшего звонок

<b>Таблица messages (информация о сообщениях):</b>
<br>id — уникальный номер сообщения
<br>message_date — дата сообщения
<br>user_id — идентификатор пользователя, отправившего сообщение

<b>Таблица internet (информация об интернет-сессиях):</b>
<br>id — уникальный номер сессии
<br>mb_used — объём потраченного за сессию интернет-трафика (в мегабайтах)
<br>session_date — дата интернет-сессии
<br>user_id — идентификатор пользователя

<b>Таблица tariffs (информация о тарифах):</b>
<br>tariff_name — название тарифа
<br>rub_monthly_fee — ежемесячная абонентская плата в рублях
<br>minutes_included — количество минут разговора в месяц, включённых в абонентскую плату
<br>messages_included — количество сообщений в месяц, включённых в абонентскую плату
<br>mb_per_month_included — объём интернет-трафика, включённого в абонентскую плату (в мегабайтах)
<br>rub_per_minute — стоимость минуты разговора сверх тарифного пакета (например, если в тарифе 100 минут разговора в месяц, то со <br>101 минуты будет взиматься плата)
<br>rub_per_message — стоимость отправки сообщения сверх тарифного пакета
<br>rub_per_gb — стоимость дополнительного гигабайта интернет-трафика сверх тарифного пакета (1 гигабайт = 1024 мегабайта)
