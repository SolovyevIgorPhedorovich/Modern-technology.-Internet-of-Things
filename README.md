# -.-
Группа: РИС-20-1бз
Соловьёв Игорь Фёдорович,
Галиуллин Евгений Валерьевич


Тема: Контроллер температуры.

Описание:
Для проекта использовался эмулятор Raspberry PI.
При помощи датчика температы DHT11, будем получать температур и влажность в комнате.
Для получения данных с датчика используется скрипт DHT11.py, которой будет запускаться командой cron каждые 5 секунд.
Данные с датчика будут отправляться на сервер post.py, и отображаться на сайте.
Для получения сигналов изменения температуры и вкл/выкл контроллера используется скрипт signal.py,
берем данные о состоянии контроллера из переменной conditioner_status, а также состояние температуры из optional_temperature и в зависимости от состояния контроллера посылаем сигнал.
