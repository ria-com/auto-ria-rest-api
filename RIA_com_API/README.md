# RIA.com


Мы начали создавать новые персонализированные API, которые помогут Вам управлять всеми Вашими обьявлениями на RIA.com

При этом, нет необходимости открывать много вкладок, теперь все API доступны в одной админ-панели. 
Зарегистрируйтесь или авторизируйтесь на [myAPI.RIA.com](http://myapi.ria.com/), чтобы использовать персонализированные API.
По умолчанию все права на доступ к сервисам не активны, что бы активировать нужный Вам сервис перейдите во вкладку "[Мої Дозволи](http://myapi.ria.com/my/credentials)"

Все методы и данные описаные с помощью стандарта DeFacto swagger 2.0


### Сервис корзина заказов 

[Полное описание сервиса  "Корзина заказов"](http://swagger.ria.com/ui/?api=/ria/basket#/basket)



#### Перечень статусов заказов

Что бы получить список типов статусов нужно отправив GET запрос на адрес [https://developers.ria.com/ria/basket/status?api_key=YOUR_API_KEY](https://developers.ria.com/ria/basket/status?api_key=YOUR_API_KEY). Результат будет примерно следующим:

 ` curl -X GET https://developers.ria.com/ria/basket/status?api_key=YOUR_API_KEY`

```javascript
{
  "status": true,
  "data": [
    {
      "id": 0,
      "name": "Новые и Невыполненные"
    },
    {
      "id": 1,
      "name": "Выполненные"
    },
    {
      "id": 2,
      "name": "Невыполненные"
    },
    {
      "id": 6,
      "name": "Удаленные"
    },
    {
      "id": 4,
      "name": "Все"
    }
  ]
}
```

#### Перечень заказов 

Что бы получить список заказов нужно отправив GET запрос на адрес [https://developers.ria.com/ria/basket/orders/?api_key=YOUR_API_KEY](https://developers.ria.com/ria/basket/orders/?api_key=YOUR_API_KEY).

 ` curl -X GET https://developers.ria.com/ria/basket/orders?api_key=YOUR_API_KEY`
 
 Результат будет примерно следующим:

```javascript
{  
   "status":true,
   "total":2,
   "orders":[  
     {  
       "order_id":21,                         // id заказа
       "status":6,                            // Статус "Удаленные"
       "total_order_sum":100,                 // Общая сумма заказа
       "created_at":"2017-04-06 16:35:31",    // Время создания
       "recipient":{  
         "user_id":000000,                    // id пользователя
         "name":"Андрій Сергійович",
         "email":"mail@gmail.com",
         "phone":"......"                     // Телефон
       },
       "delivery":{                           // Доставка
          "state_id":1,                       // id Области
         "city_id":1,                         // id Города
         "address":"Винницкая область, Винница", 
         "service":"DHL"                      // Служба доставки
       },
       "items":[  
         {  
           "adv_id":3612261,                  // id объявления
           "name":"Детали двигателя Головка блока Легковой Audi A3 Cabrio v2 v3",
           "price":100,                       // Цена
           "count":1,                         // Количество
           "note":""                          // Заметки
         }
       ]
     },
     ...
   ]
```
#### Изменение статуса заказа

Что бы изменить статус заказа нужно отправив PUT запрос на адрес` curl -X PUT "https://developers.ria.com/ria/basket/orders?user_id=*id*&order_id=*id*&api_key=YOUR_API_KEY" -H "accept: application/json" -H "content-type: application/json" -d "{ \"status\": 0}"` 
 , где *user_id* - id пользователя, *order_id* - id заказа, *status_id* - id статуса заказа, 

 
 
 Ответ будет следующим:
```javascript
{
  "status": true
}
```


## Ошибки

|  Код ошибки           | HTTP Status Code| Описание   |
|:--------------------|:--------------------------|:------------:|
|  API_KEY_MISSING |    403   | Ключ API не был указан. Подробнее об использовании ключа API см. В разделе о передаче API-интерфейса в API.    |
|  API_KEY_INVALID |    403   | Был указан недопустимый ключ API. Убедитесь, что ключ API прошел успешно, или зарегистрируйтесь для ключа API.    |
|  API_KEY_DISABLED |    403   | Ключ API был отключен администратором. Пожалуйста свяжитесь с нами для помощи.    |
|  API_KEY_UNAUTHORIZED |    403   | Предоставленный ключ API не авторизован для доступа к данной службе. Пожалуйста свяжитесь с нами для помощи.    |
|  API_KEY_UNVERIFIED |    403   | Ключ API не был подтвержден. Проверьте свой адрес электронной почты, чтобы подтвердить ключ API. Пожалуйста свяжитесь с нами для помощи.    |
|  HTTPS_REQUIRED |    400  | Запросы к этому API должны быть сделаны по протоколу HTTPS. Убедитесь, что используемый URL находится поверх HTTPS.    |
|  OVER_RATE_LIMIT |    429   | Ключ API превысил лимит запростов. Для получения дополнительной информации свяжитесь с нами.    |
|  NOT_FOUND |    404   | Не удалось найти API по данному URL-адресу. Проверьте свой URL.    |


JSON Пример
```javascript
{
  "error": {
    "code": "API_KEY_MISSING",
    "message": "No api_key was supplied. Get one at https://developers.ria.com"
  }
}
```

XML 

```xml
<response>
  <error>
    <code>API_KEY_MISSING</code>
    <message>No api_key was supplied. Get one at https://developers.ria.com</message>
  </error>
</response>
```

CSV 
```
Error Code,Error Message
API_KEY_MISSING,No api_key was supplied. Get one at https://developers.ria.com
```
HTML 

```html
<html>
  <body>
    <h1>API_KEY_MISSING</h1>
    <p>No api_key was supplied. Get one at https://developers.ria.com</p>
  </body>
</html>
```