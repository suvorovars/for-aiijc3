# Files Description

В вашем распоряжении 6 файлов:

- labled_train_data.csv - основная информация о поездке. is_aggressive - целевая переменная
- labled_train_comments.csv - комментарии за последние 2 месяца по водителям из файла labled_train_data.csv
- labled_train_tracks.csv - координаты по поездкам из файла labled_train_data.csv, собираемые трэкером раз в 60 секунд

Также мы предоставляем 3 аналогичных файла с приставкой unlabled. Для них целевую переменную мы не передаем. Мы ожидаем, что эти данные вы будете использовать для улучшения своих моделей методами semi-supervised learning.

- labled_test_data.csv,  labled_test_tracks.csv- датасеты, по которым будут проверяться решения, по ним необходимо предсказать целевую переменную is_aggressive.

# Feature Description *_train_data.csv

- order_id - id закза
- driver_id - id водителя, совершающего поездку
- client_id - id пассажира, совершающего поездку
- dttm -  дата поездки в округлении до 15 минут
- date - дата поездки в округлении до дня
- arrived_distance - дистанция, которую водитель должен преодолеть, чтобы забрать пассажира
- arrived_duration - время до точки забора пассажира
- distance - продолжительность поездки
- duration - продолжительность поездки
- from_longitude - долгота точки забора пассажира
- from_longitude - широта точки забора пассажира
- to_longitude - долгота точки прибытия пассажира
- to_latitude - широта точки прибытия пассажира
- mark - марка автомобиля, на котором совершена поездка
- client_rate_ride - оценка, которуб поставил водитель пассажиру за текущую поездку (если клиент проставил)
- client_rides_cnt - количество поездок райдера за предыдущие 30 дней, не считая поездок в текущий день

- driver_rides_cnt - количество поездок водителя за предыдущие 30 дней, не считая поездок в текущий день
- commet - комментарий к поездке при наличии
- client_rides_cnt - количество поездок райдера за предыдущие 30 дней, не считая поездок в текущий день
- is_aggressive - флаг агрессивного вождения (отсутствует для unlabled_train_tracks.csv)
