# Pizza Ordering API

Этот проект представляет собой API для заказа пицц. Он предоставляет ручки для получения информации о доступных продуктах, добавления заказов и других операций.

## Установка

1. Установите Node.js, если он не установлен на вашем компьютере.
2. Клонируйте репозиторий на свой компьютер.
3. Установите зависимости с помощью команды:

```bash
npm install
```

## Использование

Для запуска сервера выполните следующую команду:

```bash
npm start
```

По умолчанию сервер будет запущен на порту 3000. Вы можете изменить порт, задав переменной среды `PORT`.

## Ручки API

### GET /api/products

Получает список доступных продуктов (пицц) с изображениями.

Пример запроса:

```bash
GET /api/products
```

### GET /api/products/:id

Получает информацию о продукте (пицце) по его идентификатору.

Пример запроса:

```bash
GET /api/products/1
```

### GET /api/toppings

Получает список всех доступных топпингов.

Пример запроса:

```bash
GET /api/toppings
```

### POST /api/orders

Создает новый заказ.

Пример запроса:

```json
{
  "name": "John Doe",
  "phone": "123456789",
  "address": "123 Main Street",
  "paymentMethod": "credit card",
  "pizzas": [
    {
      "id": 1,
      "quantity": 2
    },
    {
      "id": 2,
      "quantity": 1
    }
  ]
}
```

## Автор

### Methed
