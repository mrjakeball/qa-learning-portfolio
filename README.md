<p>
<a href="README.md"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/ui/ru-on.svg" height="32" alt="Русский · выбран"></a>
<a href="README_EN.md"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/ui/en-off.svg" height="32" alt="English"></a>
<a href="https://github.com/mrjakeball/portfolio"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/ui/catalog-ru.svg" height="32" alt="Каталог проектов"></a>
</p>

# Практика QA с Postman

Три запроса к JSONPlaceholder показывают, как проверить существующего пользователя, отсутствующую запись и создание публикации. В экспортированной коллекции 11 проверок на JavaScript.

![GET 200 · GET 404 · POST 201](assets/social-preview.jpg)

| Запрос | Что проверяется | Проверок |
| --- | --- | ---: |
| GET · пользователь | HTTP 200, ID, имя и непустой email | 4 |
| GET · отсутствующая запись | HTTP 404 и пустой объект JSON | 2 |
| POST · публикация | HTTP 201, присвоенный ID и три отправленных поля | 5 |

## Запуск коллекции

Скачайте [JSON-файл](01-api-testing/JSONPlaceholder.postman_collection.json), импортируйте его в Postman и запустите три запроса в Collection Runner. На вкладке **Test Results** можно сверить каждую проверку с телом ответа.

Продолжение темы — [отдельная работа с PUT, PATCH и DELETE](https://github.com/mrjakeball/appsec-labs/blob/main/api-testing/01-rest-api-fundamentals/README.md).

[Профиль](https://github.com/mrjakeball) · [Каталог проектов](https://github.com/mrjakeball/portfolio)
