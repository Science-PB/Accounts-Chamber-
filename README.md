# Счетная Палата
# Решение для Кейса Аналитик со специализацией количественные исследования 

Для начала загрузим необходимые бибилиотеки и данные в формате IBM SPSS Statistics. Выведем первые 5 строчек для визульной оценки и общую информацию. Как мы видим файл состоит из 18061 строк и 747 столбцом. Данные представленны в виде category(641), float64(105), object(1). 


<img width="1051" alt="Screen Shot 2020-12-27 at 3 37 01 AM" src="https://user-images.githubusercontent.com/66921930/103167125-5cd63080-47f6-11eb-8690-0dfc917adb4e.png">



Для удобства переведем данные из category в object тип данных и выведем 5 первых строк. 


<img width="1040" alt="Screen Shot 2020-12-27 at 3 40 14 AM" src="https://user-images.githubusercontent.com/66921930/103167126-5d6ec700-47f6-11eb-844b-e33f0ae31f00.png">



В данных присутсвуют неизвестные значения (NaN) поэтому удалим их их колонки "xj1". Данные из колонки "xj1" будут использоваться для создания новой колонки под названием "Занятость". В колонке "Занятость" обьединились значения чтобы классифицировать людей по трем параметрам: "Занят", "Безработный", "Нет Ответа". Подсчитаем полученные результаты. 

<img width="1040" alt="Screen Shot 2020-12-27 at 3 41 36 AM" src="https://user-images.githubusercontent.com/66921930/103167127-5d6ec700-47f6-11eb-943e-878ed373aa05.png">




Визуализируем данные и удалим из колонки "Занятость" значения с  "Нет Ответа". 

<img width="654" alt="Screen Shot 2020-12-27 at 3 46 46 AM" src="https://user-images.githubusercontent.com/66921930/103167128-5d6ec700-47f6-11eb-8b1f-b7477cc9e01b.png">

Создадим новую колонку "Миграция" по определнным параметрам и визуализируем результат. Удалим при этом неизвестные значения. 


<img width="983" alt="Screen Shot 2020-12-27 at 3 52 00 AM" src="https://user-images.githubusercontent.com/66921930/103167311-2994a100-47f8-11eb-9ede-efc4dbffed31.png">


Удалим из колнки "Миграция" данных с значением "Нет Ответа" и создадим таблицу сопряженности для сравнения параметров "Занятость" и "Миграция". Привидем данные в этой таблице в проценты. 



<img width="622" alt="Screen Shot 2020-12-27 at 3 53 25 AM" src="https://user-images.githubusercontent.com/66921930/103167312-2ac5ce00-47f8-11eb-8128-f44854917a04.png">



Создадим теплую карту для визуализации, проведем Chi-square тест для проверки независимости переменных и выведем результат P-Value.

<img width="683" alt="Screen Shot 2020-12-27 at 3 55 42 AM" src="https://user-images.githubusercontent.com/66921930/103167313-2ac5ce00-47f8-11eb-81e6-c5d0c2aa9fed.png">



Создание новой колонки "Заработок для безработных" по критериям и ее визуализация. В аналитической записке этой части исследования нету из-за ее безпереспективности на момент аналитики. 


<img width="657" alt="Screen Shot 2020-12-27 at 3 58 10 AM" src="https://user-images.githubusercontent.com/66921930/103167314-2b5e6480-47f8-11eb-9a30-18a6668e66cf.png">



Удаление из колонки "xj60" данных с значением 'ОТКАЗ ОТ ОТВЕТА' и 'ЗАТРУДНЯЮСЬ ОТВЕТИТЬ', Создание колонки "Денег получено" с данными типа float, что даст возможность работы с числовыми данными, создание новой колонки "Прожиточный минимум" по критериям  и визуализация наблюдений.



<img width="704" alt="Screen Shot 2020-12-27 at 4 03 14 AM" src="https://user-images.githubusercontent.com/66921930/103167497-7dec5080-47f9-11eb-936d-1c93ca05304e.png">



Подсчет всех значений в колонке "Прожиточный минимум", создаем таблицу сопряженности и переводим ее в проценты.


<img width="678" alt="Screen Shot 2020-12-27 at 4 05 34 AM" src="https://user-images.githubusercontent.com/66921930/103167499-7f1d7d80-47f9-11eb-8d7c-a1f0b1aa5960.png">


Визуализация полученых данных, проведения теста и показ результата P-Value.

<img width="679" alt="Screen Shot 2020-12-27 at 4 07 34 AM" src="https://user-images.githubusercontent.com/66921930/103167500-7f1d7d80-47f9-11eb-87b7-76f4f5dc3c01.png">



Удаление из колонки "xj60" данных с значением 'ОТКАЗ ОТ ОТВЕТА' и 'ЗАТРУДНЯЮСЬ ОТВЕТИТЬ', подсчет данных для описательной статистики. 

<img width="692" alt="Screen Shot 2020-12-27 at 4 09 08 AM" src="https://user-images.githubusercontent.com/66921930/103167501-7fb61400-47f9-11eb-961d-19c34c8423e7.png">



Переименование колонки  "xh5" в "Пол", создаем таблицу сопряженности и переводим ее в проценты.


<img width="589" alt="Screen Shot 2020-12-27 at 4 15 54 AM" src="https://user-images.githubusercontent.com/66921930/103167641-dc65fe80-47fa-11eb-99f8-842aaedce9e5.png">


Визуализация полученых данных, проведения теста и показ результата P-Value.



<img width="704" alt="Screen Shot 2020-12-27 at 4 17 24 AM" src="https://user-images.githubusercontent.com/66921930/103167642-dcfe9500-47fa-11eb-95e8-7cc5d79ec793.png">



Создаем таблицу сопряженности для колонок "Занятость" и "Пол", переводим ее в проценты.

<img width="610" alt="Screen Shot 2020-12-27 at 4 19 49 AM" src="https://user-images.githubusercontent.com/66921930/103167643-dd972b80-47fa-11eb-9393-ece318e02388.png">



Визуализация полученых данных, проведения теста и показ результата P-Value.

<img width="698" alt="Screen Shot 2020-12-27 at 4 20 07 AM" src="https://user-images.githubusercontent.com/66921930/103167644-dd972b80-47fa-11eb-89b7-2480aba1aaad.png">



Создание новой таблицы с колонками "Труд_стаж", "Количество детей", "Пенсия". Очистка и подготовка данных для анализа. Показ полученой таблицы.


<img width="706" alt="Screen Shot 2020-12-27 at 4 25 24 AM" src="https://user-images.githubusercontent.com/66921930/103167749-d6245200-47fb-11eb-96dc-9cb8eeb90b1c.png">



Визуализация кореляции между переменными.


<img width="448" alt="Screen Shot 2020-12-27 at 4 25 36 AM" src="https://user-images.githubusercontent.com/66921930/103167750-d7557f00-47fb-11eb-8290-15233766b001.png">



Удаление колонки "Количесто детей" и построение гистограммы которая показывает Распределение трудового стажа. 

<img width="655" alt="Screen Shot 2020-12-27 at 4 26 09 AM" src="https://user-images.githubusercontent.com/66921930/103167751-d7ee1580-47fb-11eb-8b73-46d21efbc128.png">



Построение гистограммы которая показывает Распределение пенсий. 


<img width="654" alt="Screen Shot 2020-12-27 at 4 26 16 AM" src="https://user-images.githubusercontent.com/66921930/103167752-d886ac00-47fb-11eb-8e32-9cb8885e28e2.png">


Построение гистограммы трудового стажа для Мужчин и Женщин.


<img width="885" alt="Screen Shot 2020-12-27 at 4 30 50 AM" src="https://user-images.githubusercontent.com/66921930/103167845-ae81b980-47fc-11eb-9154-3a6104ba901c.png">


Построение гистограммы пенсии для Мужчин и Женщин.

<img width="953" alt="Screen Shot 2020-12-27 at 4 31 38 AM" src="https://user-images.githubusercontent.com/66921930/103167846-af1a5000-47fc-11eb-853d-6d7df0b0f5c1.png">


Построение точечной диаграммы для стажа и пенсии.


<img width="973" alt="Screen Shot 2020-12-27 at 4 33 01 AM" src="https://user-images.githubusercontent.com/66921930/103167847-b04b7d00-47fc-11eb-9a86-bf61c01d9e61.png">


Построение точечной диаграммы для выборки из 500 Женщин. 

<img width="794" alt="Screen Shot 2020-12-27 at 4 33 10 AM" src="https://user-images.githubusercontent.com/66921930/103167848-b0e41380-47fc-11eb-9189-70434a6f635b.png">



Создание полиномов наилучшего соответствия, это тоже не отраженно в аналитической записке. Это было сделано для сравнивания методов анализа и поиска наулучшего.

<img width="509" alt="Screen Shot 2020-12-27 at 4 34 48 AM" src="https://user-images.githubusercontent.com/66921930/103167956-8b0b3e80-47fd-11eb-810d-de103b909b7e.png">


Построение и визуализация линеной регресиии. 


<img width="671" alt="Screen Shot 2020-12-27 at 4 36 58 AM" src="https://user-images.githubusercontent.com/66921930/103167957-8ba3d500-47fd-11eb-85f1-ac26b3744ac6.png">


Создание выборки из 300 человек, построение линеной регресии для выборки. 

<img width="733" alt="Screen Shot 2020-12-27 at 4 38 08 AM" src="https://user-images.githubusercontent.com/66921930/103167958-8c3c6b80-47fd-11eb-9580-5b00c4e46957.png">


Получение наклона и точки пересечения для Мужчин и Женщин.

<img width="562" alt="Screen Shot 2020-12-27 at 4 38 40 AM" src="https://user-images.githubusercontent.com/66921930/103167959-8cd50200-47fd-11eb-8249-9a91e44428fb.png">




Предсказание значения и его проверка используя numpy и scikit learn

<img width="546" alt="Screen Shot 2020-12-27 at 4 40 46 AM" src="https://user-images.githubusercontent.com/66921930/103168027-fd7c1e80-47fd-11eb-94fc-dde6c089eb7b.png">



Подсчет коэффициента корреляции Пирсона и p-value для Мужчин и Женщин 


<img width="602" alt="Screen Shot 2020-12-27 at 4 41 54 AM" src="https://user-images.githubusercontent.com/66921930/103168028-fe14b500-47fd-11eb-8e19-8f9cc909c2c0.png">



