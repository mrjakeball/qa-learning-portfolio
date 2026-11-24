<p>
<a href="README.md"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/ui/ru-off.svg" height="32" alt="Русский"></a>
<a href="README_EN.md"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/ui/en-on.svg" height="32" alt="English · selected"></a>
<a href="https://github.com/mrjakeball/portfolio/blob/main/README_EN.md"><img src="https://raw.githubusercontent.com/mrjakeball/mrjakeball/main/assets/ui/catalog-en.svg" height="32" alt="Project catalogue"></a>
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
