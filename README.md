ПРАКТИЧЕСКОЕ ЗАДАНИЕ 18.6.1

Ваше задание: написать и протестировать Telegram-бота, в котором будет реализован следующий функционал:

<br>Бот возвращает цену на определённое количество валюты (евро, доллар или рубль).
<br>При написании бота необходимо использовать библиотеку pytelegrambotapi.
<br>Человек должен отправить сообщение боту в виде <имя валюты цену которой он хочет узнать> <имя валюты в которой надо узнать цену первой валюты> <количество первой валюты>.
<br>При вводе команды /start или /help пользователю выводятся инструкции по применению бота.
<br>При вводе команды /values должна выводиться информация о всех доступных валютах в читаемом виде.
<br>Для взятия курса валют необходимо использовать API и отправлять к нему запросы с помощью библиотеки Requests.
<br>Для парсинга полученных ответов использовать библиотеку JSON.
<br>При ошибке пользователя (например, введена неправильная или несуществующая валюта или неправильно введено число) вызывать собственно написанное исключение APIException с текстом пояснения ошибки.
<br>Текст любой ошибки с указанием типа ошибки должен отправляться пользователю в сообщения.
<br>Для отправки запросов к API описать класс со статическим методом get_price(), который принимает три аргумента: имя валюты, цену на которую надо узнать, — base, имя валюты, цену в которой надо узнать, — quote, количество переводимой валюты — amount и возвращает нужную сумму в валюте.
Т<br>окен telegramm-бота хранить в специальном конфиге (можно использовать .py файл).
<br>Все классы спрятать в файле extensions.py.
