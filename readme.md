# T-BANK Translate task

## Описание

Переводчик на основе SpringBoot и LibreTranslate

## Требования

- Java 21
- Maven
- Docker Compose

## Запуск приложения с помощью Docker

1. Склонируйте репозиторий:
    ```sh
    git clone https://github.com/annakumaneva/translate-task.git
    ```
2. Перейдите в директорию проекта:
    ```sh
    cd translate-task
    ```
3. Соберите проект с помощью Maven:
    ```sh
    mvn clean package
    ```
4. Запустите Docker Compose:
    ```sh
    docker-compose up --build
    ```

Приложение будет доступно по адресу `http://localhost:8080`.

## Использование

Для перевода строки отправьте POST-запрос на `http://localhost:8080/translate` с параметрами `text`, `from` и `to`.

Пример запроса:

```sh
curl -X POST "http://localhost:8080/translate?text=hello%20world&from=en&to=ru"

Также вы можете открыть этот адрес в браузере и также получить ответ.
