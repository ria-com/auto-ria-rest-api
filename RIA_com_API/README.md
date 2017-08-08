# RIA.com


Мы начали создавать новые персонализированные API, которые помогут Вам управлять всеми Вашими обьявлениями на RIA.com

При этом, нет необходимости открывать много вкладок, теперь все API доступны в одной админ-панели. 
Зарегистрируйтесь или авторизируйтесь на [myAPI.RIA.com](http://myapi.ria.com/), чтобы использовать персонализированные API.
По умолчанию все права на доступ к сервисам не активны, что бы активировать нужный Вам сервис перейдите во вкладку "Мої Дозволи"

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

Что бы изменить статус заказа нужно отправив PUT запрос на адрес [https://developers.ria.com/ria/basket/orders/?api_key=YOUR_API_KEY&status=status_id&order_id=_id](https://developers.ria.com/ria/basket/orders/?api_key=YOUR_API_KEY&status=status_id&order_id=_id), где 
*status_id* - id статуса заказа, *order_id* - id заказа

 ` curl -X PUT https://developers.ria.com/ria/basket/orders?api_key=YOUR_API_KEY&status=status_id&order_id=_id`
 
 Ответ будет следующим:
```javascript
{
  "status": true
}
```