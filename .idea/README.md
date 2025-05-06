Go Web Server with HTML Form
Простой веб-сервер на Go, который:

Обрабатывает GET и POST-запросы

Показывает статический HTML

Принимает данные из формы

Структура проекта
css
Копировать
Редактировать
.
├── main.go
└── static
    ├── index.html
    └── form.html
Запуск


Проверь, что в папке static/ лежат index.html и form.html.

Запусти сервер:

bash
Копировать
Редактировать
go run main.go
Сервер будет доступен по адресу: http://localhost:8080

Доступные маршруты
/ — главная страница (index.html)

/hello — простой GET-ответ "Hello!"

/form — обработка POST-формы из form.html

Пример формы
html
Копировать
Редактировать
<form method="POST" action="/form">
    <label>Name</label><input name="name" type="text"/>
    <label>Address</label><input name="address" type="text"/>
    <input type="submit" value="submit"/>
</form>
