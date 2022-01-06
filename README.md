# racing

Структура БД:
Название бд racing

Таблицы:
1) arrival - находятся все заезды (
id - идентификатор заезда
name - название заезда
race_id - номер карты (создавалась на случай, если их будет больше одной)
status - статус заезда (open, racing
racer_1 - первый гонщик
racer_2 - второй гонщик
racer_3 - третий гонщик
racer_4 - четвертый гонщик
)

2) ball - хранятся все бабки (
arrival_id - идентификатор заезда, в котором она находится
id - идентификатор бабки, приносящей очки игрокам
x	 - расположение по оси X
y - расположение по оси Y
speed_y - скорость перемещение бабки по X
speed_x скорость перемещение бабки по Y
)

3) player_killer - хранятся все полицейские (
arrival_id - идентификатор заезда, в котором он находится
id - идентификатор полицейского, убивающего игрока
x	 - расположение по оси X
y - расположение по оси Y
speed_y - скорость перемещение бабки по X
speed_x скорость перемещение бабки по Y
)

4) race - хранятся карты для заездов - не используется (не реализовано) (
id - идентификатор карты
name - название карты
data - json файл карты
)

5) racer - хранятся гонщики (
id - идентификатор гонщика
user_id - идентификатор пользователя
x - координаты по X
y - координаты по Y
angle - угол его направления
coin - заработаннные очки
life - количество жизней
)

6) users - хранятся пользователи (
id - идентификатор пользователя
name - никнейм пользователя
login - логин пользователя
password - пароль пользователя
token - токен для получения доступа к аккаунту
)
