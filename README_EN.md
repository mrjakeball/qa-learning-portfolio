<p align="center">
<a href="README.md"><picture><source media="(max-width: 600px)" srcset="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/navigation/ru-off-compact.svg?v=2"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/navigation/ru-off.svg?v=2" height="56" alt="Русский"></picture></a>
<a href="README_EN.md"><picture><source media="(max-width: 600px)" srcset="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/navigation/en-on-compact.svg?v=2"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/navigation/en-on.svg?v=2" height="56" alt="English · selected"></picture></a>
<a href="https://github.com/mrjakeball/portfolio/blob/main/README_EN.md"><picture><source media="(max-width: 600px)" srcset="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/navigation/catalog-en-compact.svg?v=2"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/navigation/catalog-en.svg?v=2" height="56" alt="Project catalogue"></picture></a>
</p>

# API testing with Postman

Three requests to JSONPlaceholder cover an existing user, a missing record and creation of a post. The exported collection contains 11 JavaScript assertions.

![GET 200 · GET 404 · POST 201](assets/social-preview.jpg)

| Request | Expected response | Assertions |
| --- | --- | ---: |
| GET · existing user | HTTP 200, ID, name and a non-empty email | 4 |
| GET · missing user | HTTP 404 and an empty JSON object | 2 |
| POST · create post | HTTP 201, assigned ID and the three submitted fields | 5 |

## Run the collection

Download the [collection JSON](01-api-testing/JSONPlaceholder.postman_collection.json), import it into Postman and run all three requests in Collection Runner. Under **Test Results**, compare individual assertions with the response body.

The [companion exercise with PUT, PATCH and DELETE](https://github.com/mrjakeball/appsec-labs/blob/main/api-testing/01-rest-api-fundamentals/README_EN.md) includes a recorded run.

[Profile](https://github.com/mrjakeball/mrjakeball/blob/main/README_EN.md) · [Project catalogue](https://github.com/mrjakeball/portfolio/blob/main/README_EN.md)
