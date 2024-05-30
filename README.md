Тестовое задание Богачев Александр Юрьевич

Урок 2
Среда разработки IntelliJ IDEA у меня установлена, JDK есть разных версий: 11, 14, 17, 21

Урок 4
Общие вопросы:
1. По вашему - кто такой QA инженер?
QA инженер - это специалист основная цель деятельности которого - оценка качества разрабатываемого программного обеспечения путём проверки соответствия продукта заявленным требованиям, сбора и передачи информации о несоответствиях.

2. Что такое тестирование?
Тестирование - это процесс проверки на соответствие реальных и ожидаемых результатов поведения программы

3. Зачем вообще проводить проверку ПО?
Проверка ПО проводится для оценки качества, проверки что ПО работает стабильно и поиска дефектов


Логическая задача:
Для того чтобы первому пирату получить максимальное количество денег и остаться в живых, ему нужно себе оставить 98 золотых, второму пирату 0, третьему пирату 1, четвертому пирату 0 и пятому пирату 1 золотой.


 
Задачи на тестирование:
1. Как протестировать сломанный тостер?
Первоначальные вопросы про тестирование тостера: 
-	Сколько у меня времени? 
-	Что это за тостер? 
-	На какой мощности он работает согласно производителю? 
-	Предоставляет ли производитель какое-либо руководство пользователя или документацию? 
-	Как это работает? 
-	Тостер с таймером или ручной? 
-	Хлеб каких размеров ему подойдет? 
-	По словам производителя, сколько времени потребуется, чтобы поджарить ломтик хлеба? 
-	Достаточно ли безопасно им пользоваться ребенку (уточнить возрастной диапазон)?


2. В приложении к тестовому заданию вы найдете 2 скриншота - реальное приложение (приложение №1) и макет (приложение №2). Найдите ошибки при реализации. Опционально - дайте рекомендации по улучшению.
Отчеты о найденных дефектах:
1: Не соответствие описания макету в верхней части экрана после заказа банковской карты
Шаги воспроизведения:
1.	Открыть приложение банка
2.	Авторизоваться в приложении
3.	Ввести данные для оформления карты
4.	Подтвердить оформление карты
Фактический результат: После подтверждения оформления карты над хлопушкой присутствует надпись «Доставка карты»

Ожидаемый результат: После подтверждения оформления карты над хлопушкой присутствует надпись «Карта готова»

2: Не соответствие описания макету в нижней части экрана после заказа банковской карты
Шаги воспроизведения:
1.	Открыть приложение банка
2.	Авторизоваться в приложении
3.	Ввести данные для оформления карты
4.	Подтвердить оформление карты
Фактический результат: После подтверждения оформления карты под хлопушкой присутствует сообщение «Доставим карту»
Ожидаемый результат: После подтверждения оформления карты под хлопушкой присутствует сообщение «Карту можно забрать»

3: Не соответствие описания макету в нижней части экрана после заказа банковской карты
Шаги воспроизведения:
1.	Открыть приложение банка
2.	Авторизоваться в приложении
3.	Ввести данные для оформления карты
4.	Подтвердить оформление карты
Фактический результат: После подтверждения оформления карты под хлопушкой в сообщении «Доставим карту» написана дата доставки
Ожидаемый результат: После подтверждения оформления карты под хлопушкой присутствует сообщение «Карту можно забрать» должна быть дата до, которой можно забрать карту

4: Не соответствие описания макету в нижней части экрана после заказа банковской карты
Шаги воспроизведения:
1.	Открыть приложение банка
2.	Авторизоваться в приложении
3.	Ввести данные для оформления карты
4.	Подтвердить оформление карты
Фактический результат: После подтверждения оформления карты под хлопушкой в сообщении «Доставим карту» надпись на кнопке «Закрыть»
Ожидаемый результат: После подтверждения оформления карты под хлопушкой в сообщении «Карту можно забрать» надпись на кнопке «Готово»


 
3. Вам передали на тестирование калькулятор и список проверок к нему, которые написал предыдущий QA. Требования описаны чуть ниже. Ваша задача - проверить корректность этих проверок.

Локализованные ошибки:
1. Тест № 1 - «1 + 1 + 1» ОР и ФР должны быть 3, а не 2.
2. Тест № 3 - «Девять целых девять десятых плюс 0,1» операция «плюсс» написана с 1 «с», должна быть с двумя (по крайней мере так описано в исходных данных).
3. Тест № 4 - в ОР стоит не правильный результат умножения 15 на 25, ОР должен быть «375 (триста семьдесят пять)».
4. Тест № 5 - различия в ОР и ФР, скорее всего связаны с тем, что в приложении не прописано округление чисел, а идет просто отсечение до 5 знаков после запятой.
5. Тест № 6 - различия в ОР и ФР, связано с отсутствием реализации операций над отрицательными числами.
6. Тест № 7 - В тестовых данных «Триста четыренадцать минус 14» опечатка в слове «четырнадцать». В требованиях  не прописано как в этом случае должна вести себя программа, скорее всего должна выдавать сообщение «Некорректный ввод».

