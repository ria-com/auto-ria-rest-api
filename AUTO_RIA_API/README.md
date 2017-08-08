

# AUTO.RIA

Для получения **API_KEY** нужно зарегестрироваться на [Developers.ria.com](https://developers.ria.com/)

```
* Наличие ссылки на сайт AUTO.RIA с гиперссылкой на страницу https://AUTO.RIA.com, 
не закрытой для индексации поисковыми системами, является единственным 
обязательным требованием для использования сервиса.
```


# API Поиска


Чтобы обратиться к  RIA API search, Вам необходимо выполнить GET запрос такого вида:

https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&PARAMETERS

или `curl -i -g -X GET "https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&PARAMETERS" '`

Он состоит из:

 * **SEARCH** — название метода API, к которому Вы хотите обратиться.

 * **API_KEY** — ключ доступа. Для получения ключа доступа нужно зарегестрироватся на портале dev.ria.com 

 * **PARAMETERS** — входные параметры, последовательность пар name=value, разделенных амперсандом. Список параметров указан  [здесь](#user-content-Список-параметров)
 

В ответ на такой запрос Вы получите ответ в формате JSON:

```javascript
[
 {
  "additional_params": {
    "lang_id": 2,                                             // Русский язык
    "page": 0,                                                // Порядеовый номер страницы
    "view_type_id": 0,
    "target": "search",
    "section": "auto",                                        // Поиск по авто
    "catalog_name": "",
    "elastica": true,
    "nodejs": true
  },
  "result": {                                                // Результат поиска
    "search_result": {
      "ids": [                                               // id объявлений
        ....
        ....
        ....
        
      ],
      "count": 11,                                          // Количество id объявлений доступных по заданым параметрам
      "last_id": 0,
      "qs": {
        "fields": [
          "_id"
        ],
        "size": 50,                                         // Количество отображаемых id объявлений
        "from": 0,  
 ]
```

## Список параметров

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|  [Тип транспорта](#user-content-Типы-транспорта)  |    сategory_id   | `Number`    |
|  [Тип кузова](#user-content-Типы-кузова)         |  body_id                  |  `Number`      |
|  [Марка](#user-content-Марки)              |  marka_id                 |  `Number`      |
|  [Модель](#user-content-Модели)             |  model_id                 |  `Number`      |
|  Год выпуска        |  yers                     |  `Number[]`  |
|  [Коробка передач](#user-content-Коробки-передач)    |  gear_id                  |  `Number[]`      |
|  [Тип топлива](#user-content-Типы-топлива)        |  type_id                  |  `Number[]`      |
|  [Тип привода](#user-content-Типы-топлива)        |  drive_id                 |  `Number`      |
|  [Опции](#user-content-Опции)              |  options                  |  `Number[]`      |
|  Пробег             |  raceInt                  |  `Number[]`  |
|  Количество дверей  |  door                     |  `Number`      |
|  [Область](#user-content-Области)            |  state_id                 |  `Number`      |
|  [Город](#user-content-Города)              |  city_id                  |  `Number`      |
|  Грузоподъемность   |  carrying                 |  `Number`      |
|  Количество мест    |  seats                    |  `Number`      |
|  [Цвет](#user-content-Цвета)               |  color_id                 |  `Number`      |
|  [Растаможка](#user-content-Растаможка)         |  custom               | `Number`         |
|  [После ДТП](#user-content-После-ДТП) | damage | `Number`|
|  [Взято в кредит](#user-content-Взято-в-кредит) | under_credit | `Number` |
|  [Конфискат](#user-content-Конфискат) | confiscated_car | `Number` |
|  [Цена от](#user-content-Цена) |price_ot |`Number[]`|
|  [Цена до](#user-content-Цена) |price_do |`Number[]`|
|  [Валюта](#user-content-Валюта) |currency |`Number`|
|  [Торг](#user-content-Торг) |auctionPossible |`Number`|
|  [Oбмен на недвижимость](#user-content-Oбмен-на-недвижимость) |with_real_exchange |`Number`|
|  [Oбмен на автомобиль](#user-content-Oбмен-на-автомобиль) |with_exchange|`Number`|
|  [Авто не в Украине ](#user-content-Авто-не-в-Украине) |abroad |`Number`|
|  [Не на ходу](#user-content-Не-на-ходу) |auto_repairs |`Number`|
|  [Продавец](#user-content-Продавец) |sellerType |`Number`|
|  [Пригнан из](#user-content-Пригнан-из) |matched_country |`Number`|
|  [Объем двигателя от](#user-content-Объем-двигателя) |engineVolumeFrom |`Number[]`|
|  [Объем двигателя до](#user-content-Объем-двигателя) |engineVolumeTo |`Number[]`|
|  [Расход топлива от](#user-content-Расход-топлива) |fuelRateFrom |`Number[]`|
|  [Расход топлива до](#user-content-Расход-топлива) |fuelRateTo |`Number[]`|
|  [Цикл](#user-content-Расход-топлива) |fuelRatesType |`String`|
|  [Мощность двигателя от](#user-content-Мощность-двигателя) |powerFrom |`Number[]`|
|  [Мощность двигателя до](#user-content-Мощность-двигателя) |powerTo |`Number[]`|
|  [Единица измерения мощности ](#user-content-Мощность-двигателя) |power_name |`Number`|
|  [Сортировка](#user-content-Сортировка) |order_by |`Number`|
|  [Период подачи](#user-content-Период-подачи) |top |`Number`|
|  [Актуальность](#user-content-Актуальность) |saledParam |`Number`|
|  [VIN код](#user-content-VIN-код) |verified.VIN |`Number`|
|  [Колесная формула](#user-content-Колесная-формула) |wheelFormulaId |`Number`|
|  [Количество осей](#user-content-Количество-осей) |axleId |`Number`|
|  [Фото](#user-content-Только-с-Фото ) |with_photo |`Number`|
|  [Видео](#user-content-Только-с-Видео) |with_video |`Number`|
|  [Количество отображаемых id](#user-content-Количество-отображаемых-id) |countpage |`Number`|
|  [Номер страницы](#user-content-Номер-страницы) |page |`Number`|

## Пример

Допустим Вы ищете:

* Легковые машины                                            ``(сategory_id=1)``
* Кузов *Седан*,*Универсал*                                 `(bodystyle[0]=3&bodystyle[4]=2)`
* Япония                                                   `(brandOrigin[0]=276)`
    * Toyota                                               ` (marka_id[0]=79)`
    * Все модели                                            `(model_id[0]=0)`
    * Год выпуска от 2010 по 2017г.                        ` (s_yers[0]=2010&po_yers[0]=2017)`
* Германия                                                  `(brandOrigin[1]=392)`
    * Volkswagen                                            `(marka_id[1]=84)`
    * Все модели                                            `(model_id[1]=0)`
    * Год выпуска от 2012 по 2016г.                        `(s_yers[1]=2012&po_yers[1]=2016)`      
* Цена от 1000 до 60000                                     `(price_ot=1000&price_do=60000)`
    * Цена указана в доларах США                           ` (currency=1)`
* Возможен торг                                             `(auctionPossible=1)`
* Возможен обмен на недвижимость                           ` (with_real_exchange=1)`
* Возможен обмен на автомобиль                             ` (with_exchange=1)`
    * Марка автомобиля любая                               ` (exchange_filter[marka_id]=0)`
    * Модель автомобиля любая                              ` (exchange_filter[model_id]=0)`
* Область
    * Винницкая - поиск по всем городам этой области       ` (state[0]=1&city[0]=0)`
    * Житомирская - поиск по всем городам этой области     ` (state[1]=2&city[1]=0)`
    * Киевская - поиск по всем городам этой области        ` (state[2]=10&city[2]=0)`
* Не отображать авто которые находяться не в Украине       ` (abroad=2)`
* Не отображать нерастаможенные авто                       ` (custom=1)`
* Гаражное хранение                                         `(auto_options[477]=477)`
* Топливо
    * Бензин                                                `(type[0]=1)`
    * Дизель                                                `(type[1]=2)`
    * Газ/бензин                                            `(type[3]=4)`
    * Электро                                               `(type[5]:6)`
* КПП
    * Ручная / Механика                                     `(gearbox[0]=1)`
    * Автомат                                               `(gearbox[1]=2)`
    * Типтроник                                             `(gearbox[2]=3)`
* Объем 1.4 - 3.2 л.                                        `(engineVolumeFrom=1.4&engineVolumeTo=3.2)`
* Мощность 90 - 250                                         `(powerFrom=90&powerTo=250)`
    * Единица измерения мощности - л.с                      `(power_name=1)`
* Только с фото                                             `(with_photo=1)`

В итоге мы получаем запрос такого [вида]:

[https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&category_id=1&bodystyle[0]=3&....][1] 

[1]:https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&category_id=1&bodystyle[0]=3&bodystyle[4]=2&marka_id[0]=79&model_id[0]=0&s_yers[0]=2010&po_yers[0]=2017&marka_id[1]=84&model_id[1]=0&s_yers[1]=2012&po_yers[1]=2016&brandOrigin[0]=276&brandOrigin[1]=392&price_ot=1000&price_do=60000&currency=1&auctionPossible=1&with_real_exchange=1&with_exchange=1&exchange_filter[marka_id]=0&exchange_filter[model_id]=0&state[0]=1&city[0]=0&state[1]=2&city[1]=0&state[2]=10&city[2]=0&abroad=2&custom=1&auto_options[477]=477&type[0]=1&type[1]=2&type[3]=4&type[7]=8&gearbox[0]=1&gearbox[1]=2&gearbox[2]=3&engineVolumeFrom=1.4&engineVolumeTo=3.2&powerFrom=90&powerTo=250&power_name=1&countpage=50&with_photo=1                                

В случае успешного выполнения запроса по указанным параметрам результат будет со статусом **200 OK**.

Пример успешного ответа:
```javascript
[
    {
   "additional_params": {
     "lang_id": 2,                                  // Русский язык
     "page": 0,                                     // Порядеовый номер страницы
     "view_type_id": 0,
     "target": "search",
     "section": "auto",                             // Поиск по авто
     "catalog_name": "",
     "elastica": true,
     "nodejs": true
   },
   "result": {                                      // Результат поиска
     "search_result": {
       "ids": [
         "19519211",
         "19684763",
         "19493489",
         "19714833",
         "19393702",
         "19692238",                                // id объявлений
         "19574398",
         "18154136",
         "19391327",
         "18693600",
         "19431563",
         "18047892"
       ],
       "count": 1,                                 // Количество id объявлений доступных по заданым параметрам
       "last_id": 0, 
       "qs": {
         "fields": [
           "_id"
         ],
         "size": 50,                                // Количество отображаемых id объявлений
         "from": 0,
             } 
            }     
           }
   }   
 ]
```


**Важно**

Максимальное количество отображаемых id объявлений за один запрос равно 100(*countpage*).В случае если результат 
поиска превышает это значение можно добавить параметр *page* (порядковый номер страницы) c помощью которго можно 
просматреть все результаты поиска.

```
"additional_params": {
    "lang_id": 2,
    "page": "1",                           // Порядковый номер страницы     
    "view_type_id": 0,
    "target": "search",
    "section": "auto",
    "catalog_name": "",
    "elastica": true,
    "nodejs": true
  },
  "result": {
    "search_result": {
      "ids": [
        "19885907",
        "19885290",
        "19847856",
        "19876230",
        "19662019",
        "18493054",
        "19440597",
        "19865852",
        "18814906",
        "19862470",
        "19738583",
       . . . . . . .     
        "19860637",
        "19747721",
        "18050784",
        "19810589",
        "19746765",
        "18412097",
        "18545537"
      ],
      "count": 1578,                         // Количество id по результатам поиска
      "last_id": 0,
      "qs": {
        "fields": [
          "_id"
        ],
        "size": 100,
        "from": 100,
```

Параметры поиска на сайте AUTO.RIA отличаются от параметров указанных ниже. Для использования параметров поиска с сайта AUTO.RIA
нужно обратиться к сервису конфигурации новых параметров в старые.

*Пример*

Допустим Вам нужен список автомобилей по параметрам указаных ниже:

[https://auto.ria.com/search/?categories.main.id=1&brand.id[0]...][2]

[2]:https://auto.ria.com/search/?categories.main.id=1&brand.id[0]=9&year[0].gte=2011&year[0].lte=2016&custom.not=1&fuel.id[5]=6&gearbox.id[1]=2&gearbox.id[2]=3&size=10"&countpage=100

Используем сервис конфигурации

[https://developers.ria.com/new_to_old?api_key=YOUR_API_KEY&categories.main.id=1&brand.id...][3]

[3]:https://developers.ria.com/new_to_old?api_key=YOUR_API_KEY&categories.main.id=1&brand.id[0]=9&year[0].gte=2011&year[0].lte=2016&custom.not=1&fuel.id[5]=6&gearbox.id[1]=2&gearbox.id[2]=3&size=10"&countpage=10

В результате мы получим параметры которые сможем применять в API Search:
```json
{
  "unrecognized": {
    "countpage": "100"
  },
  "converted": {
    "category_id": "1",
    "marka_id[0]": "9",
    "model_id[0]": "0",
    "s_yers[0]": "2011",
    "po_yers[0]": "2016",
    "custom": "1",
    "type[5]": "6",
    "gearbox[1]": "2",
    "gearbox[2]": "3",
    "countpage": "10\""
  },
  "string": "category_id=1&marka_id%5B0%5D=9&model_id%5B0%5D=0&s_yers%5B0%5D=2011&po_yers%5B0%5D=2016&custom=1&type%5B5%5D=6&gearbox%5B1%5D=2&gearbox%5B2%5D=3&countpage=10%22"
}

```
Этот запрос можно производить и в обратном порядке:

Используем сервис конфигурации

[https://developers.ria.com/old_to_new?api_key=YOUR_API_KEY&category_id=1&marka_id[0]=9...][4]

[4]:https://developers.ria.com/old_to_new?api_key=YOUR_API_KEY&category_id=1&marka_id[0]=9&model_id[0]=0&s_yers[0]=2011&po_yers[0]=2016&custom=1&type[5]=6&gearbox[1]=2&gearbox[2]=3&countpage=100

В результате мы получим новые параметры которые можем использовать на сайте AUTO.RIA
```json
{
  "unrecognized": {
    
  },
  "converted": {
    "categories.main.id": "1",
    "brand.id[0]": "9",
    "year[0].gte": "2011",
    "year[0].lte": "2016",
    "custom.not": "1",
    "fuel.id[5]": "6",
    "gearbox.id[1]": "2",
    "gearbox.id[2]": "3",
    "size": "100"
  },
  "string": "categories.main.id=1&brand.id%5B0%5D=9&year%5B0%5D.gte=2011&year%5B0%5D.lte=2016&custom.not=1&fuel.id%5B5%5D=6&gearbox.id%5B1%5D=2&gearbox.id%5B2%5D=3&size=100"
}
```

**Так же на основе этого веб-сервиса был создан экспериментальный Telegram-бот написанный на Node.js, детальней 
с ним можно ознакомиться [здесь](https://github.com/ria-com/api_autoria_search_bot)**

# AUTO info  Информация по id объявления

Чтобы обратиться к  RIA API info, Вам необходимо выполнить GET запрос такого вида:

https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=**id_объявления**

или  `curl -i -X GET "https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=id_объявления"`

Он состоит из:

 * **info** — название метода API, к которому Вы хотите обратиться.
 
 * **API_KEY** — ключ доступа. Для получения ключа доступа нужно зарегестрироватся на портале developers.ria.com 

 * **auto_id=** — номер объявления по которому нужна информация
 
## Пример

Допусти Вам нужна информация по _19050985_ id.

Данный запрос будет выглядеть так:

https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=19050985

или  `curl -i -X GET "https://developers.ria.com/auto/info?api_key=YOUR_API_KEY&auto_id=19050985"`

В случае успешного выполнения запроса  результат будет со статусом **200 OK**.

Пример успешного ответа:

```javascript
[
 {
  "userId": 489269,                                                                       // id пользователя
  "chipsCount": 0,
  "locationCityName": "Днепропетровск",                                                   // Город
  "auctionPossible": false,                                                               // Торг 
  "exchangePossible": false,                                                              // Обмен    
  "realtyExchange": false,                                                                // Обмен на надвижимость 
  "exchangeType": "Любой",                                                                // Тип обмена
  "exchangeTypeId": 0,                                                                    // Идентификатор типа обмена
  "addDate": "2017-04-24 23:02:06",                                                       // Дата и время добавления 
  "updateDate": "2017-04-24 23:02:06",                                                    // Дата и время обновления 
  "expireDate": "2017-07-24 23:02:06",                                                    // Дата и время истечения
  "userHideADSStatus": false,                                                             // Пользователь скрыл статус
  "userPhoneData": {
    "phoneId": "3336492",                                                                 // id телефона пользователя 
    "phone": "(067) 522-60-77"                                                            // Телефон пользователя
  },
  "USD": 33500,                                                                           // Стоимость в доларах США
  "UAH": 880380,                                                                          // Стоимость в гривнах
  "EUR": 30815,                                                                           // Стоимость в евро
  "isAutoAddedByPartner": false,                                                          
  "partnerId": 0, 
  "levelData": {
    "level": 10,                                                                          // Уровень топа
    "label": 3,                                                                           // Метка
    "hotType": "срочно",                                                                  // Метка "TOP" или "Срочно"
    "expireDate": "2017-05-04 23:02:07"                                                   // Дата и время истечения метки "тор" "Срочно"
  },
  "autoData": {                                                                           // Характеристики машины
    "description": "Итак. Пришло время в срочном порядке продать свой любимый автомобиль. " +
     "\r\nПокупал его в августе 2013 года. \r\nПолностью обслужен на о",                  // Описание
    
    "version": "",
    "onModeration": false,
    "year": 2013,                                                                         // Год выпуска
    "autoId": 19050985,                                                                   // id объявления
    "statusId": 0,                                                                        //  - 
    "withVideo": false,                                                                   // Наличие видео                               
    "race": "60 тыс. км",                                                                 // Пробег
    "raceInt": 60,                                                                        // - 
    "fuelName": "Дизель",                                                                 // Тип топлива
    "gearboxName": "Автомат",                                                             // Тип привода
    "isSold": false,                                                                      // Этот параметр показывает или машына продана или нет
    "mainCurrency": "USD",                                                                // Основная валюта
    "fromArchive": false,
    "categoryId": 1,                                                                      // Тип транспорта
    "custom": 0                                                                           
  },
  "markName": "Volvo",                                                                    // Марка автомобиля
  "markId": 85,                                                                           // id марки автомобиля
  "modelName": "XC90",                                                                    // Модель автомобиля
  "modelId": 824,                                                                         // id Модели автомобиля
  "photoData": {                                                                          // Фотографии
    "count": 15,                                                                          // Количество фотографий
    "seoLinkM": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196m.jpg",
    "seoLinkSX": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196sx.jpg",
    "seoLinkB": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196b.jpg",
    "seoLinkF": "https://cdn.riastatic.com/photosnew/auto/photo/volvo_xc90__181949196f.jpg"
  },
  "linkToView": "/auto_volvo_xc90_19050985.html",                                         // Линк на объявление
  "title": "Volvo XC90",                                                                  // Название
  "stateData": {                                     
    "name": "Днепропетровск",                                                             // Город
    "regionName": "Днепропетровская",                                                     // Область
    "linkToCatalog": "/city/dnepropetrovsk/",
    "title": "Поиск объявлений по городу Днепропетровск",
    "stateId": 11                                                                         // id Города
  },
  "oldTop": {
    "isActive": true,
    "expireDate": ""
  },
  "canSetSpecificPhoneToAdvert": false,
  "dontComment": 0,
  "sendComments": 0,
  "badges": [
    
  ],
  "checkedVin": {                                                                        // Проверка vin-кода
    "isShow": false,                                                                     // Отображать vin-код
    "linkToReport": "/vin-check/auto/19050985/",
    "hasRestrictions": false,                                                            // Ограничения
    "checkDate": "04.05.2017",
    "isChecked": false                                                                  //  vin-код проверен
  },
  "isLeasing": 0,   // Лизинг 
  "dealer": {
    "link": "",
    "logo": "",
    "type": "",
    "id": 0,
    "name": "",
    "packageId": 0,
    "typeId": 0
  },
  "withInfoBar": false,                                                                // Информационная панель
  "infoBarText": "",
  "optionStyles": [
    
  ]    
]
 ```  
 
 # Подсчёт средней цены
 
 **“Подсчёт средней цены”** — 
 первый сервис, основанный на актуальных статистических данных **AUTO.RIA** (ежемесячно 10 тыс. опубликованных объявлений о продаже 7 800 марок авто, которые ежедневно собирают 8 млн. просмотров).
 
 Теперь вы можете:
 * узнавать актуальные средние цены автомобилей разных марок и моделей; 
 * следить за изменениями цен в кратко- и долгосрочном периодах;
 * анализировать и прогнозировать изменения цен и спроса на автомобили;
 * размещать полученную информацию на вашем сайте.`*`
 
 ```
 * Наличие ссылки на сайт AUTO.RIA с гиперссылкой на страницу https://AUTO.RIA.com, 
 не закрытой для индексации поисковыми системами, является единственным 
 обязательным требованием для использования сервиса.
 ```
 
 Ознакомьтесь с технической документацией, чтобы получить доступ и экспортировать необходимую информацию в программу вашей компании.
 
 Благодарим за содействие в запуске сервиса “Подсчёт средней цены” ТОВ «Богдан–Авто Холдинг».
 
 Ваш AUTO.RIA, автосайт № 1 в Украине.
 
### Формат данных в запросе

Все параметры описанные в таблице поддерживаемых параметров должны передаватся в виде чисел. Исключениями являются только параметры - *год выпуска*. *пробег*, *опции* и *коробка передач*.

Если передать массив в параметре *коробка передач*, то это будет интерпретироваться как поиск коробок передач с логическим оператором *ИЛИ*. Т.е. `https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&marka_id=9&model_id=31612&gear_id=1&gear_id=2` - выберет для подсчета все **BMW 318** с автоматическими и ручными коробками передач. Аналогично и с параметром *тип топлива*, например: `https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&marka_id=9&model_id=31887&yers=2014&fuel_id=1&fuel_id=2` - выберет для подсчета все **BMW 520 2014 года** с дизельными и бензиновыми двигателями.  

Если передать массив в параметре *год выпуска* или *пробег* это будет интерпретироваться как диапазон значений. Например, `https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&raceInt=10&raceInt=100` - выберет для подсчета средней цены все объявления с пробегом от 10 до 100 тыс. км.

Если передать массив значений в параметре *опции* это будет интерпретироваться как поиск опций с логическим оператором "И". Т.е. `https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&options=217&options=463` выберет для подсчета все объявления, у которых есть опция *ABS* **И** *Галогенные фары*.

### Формат данных в ответе

В случае успешного подсчета средней цены по указанным параметрам результат будет со статусом **200 OK**.

Пример успешного ответа:
```javascript
{
    total: 17,
    arithmeticMean: 16305.882352941177,
    interQuartileMean: 8483.333333333334,
    percentiles: {
        1.0: 1944,
        5.0: 2520,
        25.0: 3500,
        50.0: 8000,
        75.0: 23500,
        95.0: 53539.999999999985,
        99.0: 64868
    },
    prices: [
        67700,
        27000,
        3000,
        23500,
        3500,
        8100,
        10000,
        3500,
        2700,
        8000,
        11000,
        45800,
        50000,
        1800,
        4350,
        4400,
        2850
    ],
    classifieds: [
        14663610,
        14226353,
        14138132,
        13969588,
        14697569,
        13386778,
        13279188,
        14555863,
        14754932,
        14816842,
        14664706,
        13873344,
        14681607,
        14772056,
        14059841,
        14290096,
        14890250
    ]
}
```
Расшифровка параметров:
- *total* - общее количество объявлений, учавствующих в подсчете.
- *arithmeticMean* - [среднее арифметическое](https://ru.wikipedia.org/wiki/%D0%A1%D1%80%D0%B5%D0%B4%D0%BD%D0%B5%D0%B5_%D0%B0%D1%80%D0%B8%D1%84%D0%BC%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%BE%D0%B5).
- *interQuartileMean* - среднее арифметическое из значений, находящихся между первым и четвертым [квантилем](https://ru.wikipedia.org/wiki/%D0%9A%D0%B2%D0%B0%D0%BD%D1%82%D0%B8%D0%BB%D1%8C). Грубо говоря, это среднее арифметическое без учета 25% самых маленьких и самых больших значений.
- *percentiles* - значения [процентилей](https://ru.wikipedia.org/wiki/%D0%9A%D0%B2%D0%B0%D0%BD%D1%82%D0%B8%D0%BB%D1%8C#.D0.9F.D0.B5.D1.80.D1.86.D0.B5.D0.BD.D1.82.D0.B8.D0.BB.D1.8C). Т.е. для данного примера 25% всех объявлений имеют цену ниже $3500.
- *prices* - список цен, которые учавствовали в подсчете средней цены. Размер ограничен 1000 элементов.
- *classifieds* - идентификаторы объявлений, к которым принадлежат цены соответственно. Размер ограничен 1000 элементов.

Записи в поля "classifields" и "prices" идут в одинаковом порядке.

Если по каким-либо причинам не удалось подсчитать среднюю цену, ответ будет иметь статус **400 Bad Request**, а тело ответа будет содержать следующее:
```javascript
{ "message": "Not Enough Data" }
```

### Примеры

Средняя цена по BMW X5 с пробегом от 10 до 100 тыс. км. - [https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&marka_id=9&model_id=96&raceInt=10&raceInt=100](https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEYd&marka_id=9&model_id=96&raceInt=10&raceInt=100).


Средняя цена для Honda Accord в Киеве - [https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&marka_id=28&model_id=262&city_id=9](https://developers.ria.com/auto/average_price?api_key=YOUR_API_KEY&marka_id=28&model_id=262&city_id=9)
 
 
 
 
 
 
## Методы для работы с Параметрами

### Типы транспорта

Что бы получить список типов транспорта нужно отправив GET запрос на адрес [https://developers.ria.com/auto/categories/?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/?api_key=YOUR_API_KEY). Результат будет примерно следующим:
```javascript
[
    { name: "Легковые", value: 1 },
    { name: "Мото", value: 2 },
    { name: "Водный транспорт", value: 3 },
    { name: "Спецтехника", value: 4 },
    { name: "Прицеп", value: 5 },
    { name: "Грузовик", value: 6 },
    { name: "Автобус", value: 7 },
    { name: "Автодом", value: 8 },
    { name: "Воздушный транспорт", value: 9 }
]
```

### Типы кузова

Типы кузова зависят от типов транспорта. Поэтому для того, чтобы получить список типов кузова необходимо отправить GET запрос на адрес `https://developers.ria.com/auto/categories/:categoryId/bodystyles?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта, *api_key*- Ваш ключ.

Например, для легковых автомобилей ([https://developers.ria.com/auto/categories/1/bodystyles?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/bodystyles?api_key=YOUR_API_KEY)), результат будет следующим:
```javascript
[
    { name: "Седан", value: 3 },
    { name: "Внедорожник / Кроссовер", value: 5 },
    { name: "Минивэн", value: 8 },
    { name: "Хэтчбек", value: 4 },
    { name: "Универсал", value: 2 },
    { name: "Купе", value: 6 },
    { name: "Легковой фургон (до 1,5 т)", value: 254 },
    { name: "Кабриолет", value: 7 },
    { name: "Пикап", value: 9 },
    { name: "Лимузин", value: 252 },
    { name: "Другой", value: 28 }
]
```

Также типы кузова могут быть разделены на группы. Это актуально для спецтехники. Поэтому существует способ получить сгруппированные типы кузова отправив GET запрос по адресу `https://developers.ria.com/auto/categories/:categoryId/bodystyles/_group?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта, *api_key*- Ваш ключ.

Например, для мотоциклов ([https://developers.ria.com/auto/categories/2/bodystyles/_group?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/bodystyles/_group?api_key=YOUR_API_KEY)), результат будет следующим:
```javascript
[
    [
        { name: "Мопеды", value: 58 },
        { name: "Скутер / Мотороллер", value: 11 },
        { name: "Макси-скутер", value: 12 }
    ],
    [
        { name: "Мотоциклы", value: 13 },
        { name: "Мотоцикл Без обтекателей (Naked bike)", value: 15 },
        { name: "Мотоцикл Внедорожный (Enduro)", value: 21 },
        { name: "Мотоцикл Кастом", value: 30 },
        { name: "Мотоцикл Классик", value: 14 },
        { name: "Мотоцикл Кросс", value: 19 },
        { name: "Мотоцикл Круизер", value: 24 },
        { name: "Мотоцикл Многоцелевой (All-round)", value: 25 },
        { name: "Мотоцикл с коляской", value: 29 },
        { name: "Спортбайк", value: 18 },
        { name: "Мотоцикл Спорт-туризм", value: 17 },
        { name: "Мотоцикл Супермото (Motard)", value: 22 },
        { name: "Мотоцикл Триал", value: 20 },
        { name: "Мотоцикл Туризм", value: 16 },
        { name: "Мотоцикл Чоппер", value: 23 }
    ],
    [
        { name: "Мини мотоциклы", value: 31 },
        { name: "Мини спорт", value: 32 },
        { name: "Мини крос (Питбайк)", value: 33 }
    ],
        { name: "Трицикл", value: 34 },
        { name: "Трайк", value: 57 },
    [
        { name: "Квадроциклы", value: 35 },
        { name: "Квадроцикл детский", value: 36 },
        { name: "Квадроцикл спортивный", value: 39 },
        { name: "Квадроцикл утилитарный", value: 41 },
        { name: "Мотовездеход", value: 42 },
        { name: "Вездеход-амфибия", value: 43 },
        { name: "Гольф-кар", value: 44 },
        { name: "Картинг", value: 45 }
    ],
    { name: "Снегоход", value: 46 },
    { name: "Другое", value: 56 }
]
```

Формат данных при этом отличается от обычного - это коллекция объектов, в которой есть другие коллекции. Группа типов кузовов всегда начинается с её названия. Например, в группу *Квадроциклы* входят типы кузовов *Квадроцикл детский*, *Квадроцикл спортивный*, *Квадроцикл утилитарный*, *Мотовездеход* и т.д.

Также, при необходимости, можно получиться просто весь список типов кузовов, послав GET запрос по адресу [https://developers.ria.com/auto/bodystyles?api_key=YOUR_API_KEY](https://developers.ria.com/auto/bodystyles?api_key=YOUR_API_KEY).

## Методы для работы с марками и моделями

### Марки

Марки зависят от типов транспорта. Поэтому для того, чтобы получить список марок необходимо отправить GET запрос по адресу `https://developers.ria.com/auto/categories/:categoryId/marks?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта, *api_key*- Ваш ключ.

Например, для легковых автомобилей ([https://developers.ria.com/auto/categories/1/marks?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/marks?api_key=YOUR_API_KEY)), результат будет следующим:
```javascript
[
    { name: "Acura", value: 98 },
    { name: "Adler", value: 2396 },
    { name: "Aixam", value: 2 },
    { name: "Alfa Romeo", value: 3 },
    { name: "Alpine", value: 100 },
    { name: "Altamarea", value: 3988 },
    { name: "Aro", value: 101 },
    { name: "Artega", value: 3105 },
    { name: "Asia", value: 4 },
    { name: "Aston Martin", value: 5 },
    { name: "Audi", value: 6 },
    { name: "Austin", value: 7 },
    { name: "Autobianchi", value: 102 }
    ...
]
```

### Модели

Модели зависят от типов транспорта и марок. Следовательно список марок можно получить по адресу `http://api.auto.ria.com/categories/:categoryId/marks/:markId/models?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта а *markId* - идентификатор марки, *api_key*- Ваш ключ.

Например, для мотоциклов BMW ([https://developers.ria.com/auto/categories/2/marks/9/models?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/marks/9/models?api_key=YOUR_API_KEY)), список моделей будет следующим:
```javascript
[
    { name: "Adventure", value: 25290 },
    { name: "C", value: 25291 },
    { name: "CS", value: 25292 },
    { name: "DKW", value: 28318 },
    { name: "F", value: 25293 },
    { name: "G", value: 29468 },
    { name: "GS", value: 25295 },
    { name: "HP", value: 38148 },
    { name: "Independent", value: 25297 },
    { name: "K", value: 25298 },
    { name: "LT", value: 25299 },
    { name: "R", value: 25300 },
    { name: "RS", value: 32736 },
    { name: "RT", value: 25301 },
    { name: "S", value: 25302 },
    { name: "X", value: 42030 }
]
```

Модели, также как и типы кузовов, могут быть сгруппированы. Чтобы получить такой список, необходимо отправить запрос по адресу `https://developers.ria.com/auto/categories/:categoryId/marks/:markId/models/_group?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта а *markId* - идентификатор марки, *api_key*- Ваш ключ.

Например, для легковых автомобилей BMW ([https://developers.ria.com/auto/categories/1/marks/9/models/_group?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/marks/9/models/_group?api_key=YOUR_API_KEY)), список моделей будет следующим:
```javascript
[
    [
        { name: "1 Series (все)", value: 2161 },
        { name: "116", value: 34670 },
        { name: "118", value: 34671 },
        { name: "120", value: 34672 },
        { name: "123", value: 34673 },
        { name: "125", value: 34674 },
        { name: "130", value: 34675 },
        { name: "135", value: 34676 }
    ],
    [
        { name: "3 Series (все)", value: 3219 },
        { name: "3 Series GT", value: 43029 },
        { name: "315", value: 37454 },
        { name: "316", value: 30851 },
        { name: "318", value: 31612 },
        { name: "320", value: 31611 },
        { name: "321", value: 37389 },
        { name: "323", value: 34677 },
        { name: "324", value: 30687 },
        { name: "325", value: 29713 },
        { name: "326", value: 44061 },
        { name: "328", value: 31661 },
        { name: "330", value: 34678 },
        { name: "335", value: 34679 },
        { name: "340", value: 35568 }
    ],
    ...
    { name: "Alpina", value: 906 },
    { name: "Dixi", value: 33383 },
    { name: "I3", value: 44838 },
    { name: "I8", value: 44537 },
    { name: "Isetta", value: 32380 },
    { name: "Z1", value: 97 },
    { name: "Z3", value: 98 },
    { name: "Z4", value: 99 },
    { name: "Z8", value: 100 }
]
```
Формат данных такой же как и в случае с типа кузова - коллекция объектов, в которой могут быть другие объекты. Группа моделей всегда начинается с её названия.

Также, при необходимости, можно просто получить список всех моделей, отправив GET запрос по адресу [https://developers.ria.com/auto/models?api_key=YOUR_API_KEY](https://developers.ria.com/auto/models?api_key=YOUR_API_KEY).

## Методы для работы с областями и городами

### Области

Получить список областей можно отправив GET запрос по адресу [https://developers.ria.com/auto/states?api_key=YOUR_API_KEY](https://developers.ria.com/auto//states?api_key=YOUR_API_KEY).

Результат будет следующим:
```javascript
[
    { name: "Винницкая", value: 1 },
    { name: "Волынская", value: 18 },
    { name: "Днепропетровская", value: 11 },
    { name: "Донецкая", value: 13 },
    { name: "Житомирская", value: 2 },
    { name: "Закарпатская", value: 22 },
    { name: "Запорожская", value: 14 },
    { name: "Ивано-Франковская", value: 15 },
    { name: "Киевская", value: 10 },
    { name: "Кировоградская", value: 16 },
    { name: "Луганская", value: 17 },
    { name: "Львовская", value: 5 },
    { name: "Николаевская", value: 19 },
    { name: "Одесская", value: 12 },
    { name: "Полтавская", value: 20 },
    { name: "Республика Крым", value: 21 },
    { name: "Ровенская", value: 9 },
    { name: "Сумская", value: 8 },
    { name: "Тернопольская", value: 3 },
    { name: "Харьковская", value: 7 },
    { name: "Херсонская", value: 23 },
    { name: "Хмельницкая", value: 4 },
    { name: "Черкасская", value: 24 },
    { name: "Черниговская", value: 6 },
    { name: "Черновицкая", value: 25 }
]
```

### Города

Города зависят от областей, поэтому, чтобы получить их список, необходимо послать GET запрос по адресу `https://developers.ria.com/auto/states/:stateId/cities?api_key=YOUR_API_KEY`, где *stateId* - идентификатор области, *api_key*- Ваш ключ.

Например, для Винницкой области ([https://developers.ria.com/auto/states/1/cities?api_key=YOUR_API_KEY](https://developers.ria.com/auto/states/1/cities?api_key=YOUR_API_KEY)) список городов будет следующим:
```javascript
[
    { name: "Винница", value: 1 },
    { name: "Жмеринка", value: 27 },
    { name: "Казатин", value: 30 },
    { name: "Крыжополь", value: 31 },
    { name: "Липовец", value: 32 },
    { name: "Литин", value: 33 },
    { name: "Могилев-Подольский", value: 34 },
    { name: "Мурованые Куриловцы", value: 35 },
    { name: "Немиров", value: 36 },
    { name: "Оратов", value: 37 },
    { name: "Песчанка", value: 38 },
    { name: "Погребище", value: 39 },
    { name: "Теплик", value: 40 },
    { name: "Тывров", value: 41 },
    { name: "Томашполь", value: 42 },
    { name: "Тростянец", value: 43 },
    { name: "Тульчин", value: 44 },
    { name: "Хмельник", value: 45 },
    { name: "Черновцы", value: 46 },
    { name: "Чечельник", value: 47 },
    { name: "Шаргород", value: 48 },
    { name: "Ямполь", value: 49 },
    { name: "Бар", value: 597 },
    { name: "Бершадь", value: 599 },
    { name: "Гайсин", value: 602 },
    { name: "Ильинцы", value: 603 },
    { name: "Калиновка", value: 604 },
    { name: "Гнивань", value: 609 },
    { name: "Ладыжин", value: 644 }
]
```

## Методы для работы с техническими характеристиками

### Коробки передач

Коробки передач зависят от типа транспорта, поэтому, чтобы получить их список, необходимо послать GET запрос по адресу `https://developers.ria.com/auto/categories/:categoryId/gearboxes?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта, *api_key*- Ваш ключ .

Например, список коробок передач для мотоциклов ([https://developers.ria.com/auto/categories/2/gearboxes?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/gearboxes?api_key=YOUR_API_KEY)) будет выглядеть следующим образом:
```javascript
[
    { name: "Ручная / Механика", value: 1 },
    { name: "Автомат", value: 2 },
    { name: "Типтроник", value: 3 },
    { name: "Адаптивная", value: 4 },
    { name: "Вариатор", value: 5 }
]
```

### Типы привода

Типы привода также зависят от тиа транспорта, поэтому, чтобы получить их список, необходимо плсать GET запрос по адресу `https://developers.ria.com/auto/categories/:categoryId/driverTypes?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта, *api_key*- Ваш ключ.

Например, список типов привода для мотоциклов ([https://developers.ria.com/auto/categories/2/driverTypes?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/2/driverTypes?api_key=YOUR_API_KEY)) выглядит следующим образом:
```javascript
[
    { name: "Кардан", value: 4 },
    { name: "Ремень", value: 5 },
    { name: "Цепь", value: 6 }
]
```

### Типы топлива

Типы топлива можно получить отправив GET запрос по адресу [https://developers.ria.com/auto/type?api_key=YOUR_API_KEY](https://developers.ria.com/auto/type?api_key=YOUR_API_KEY). Ответ будет выглядеть так:
```javascript
[
    { name: "Бензин", value: 1 },
    { name: "Дизель", value: 2 },
    { name: "Газ", value: 3 },
    { name: "Газ/бензин", value: 4 },
    { name: "Гибрид", value: 5 },
    { name: "Электро", value: 6 },
    { name: "Другое", value: 7 },
    { name: "Газ метан", value: 8 },
    { name: "Газ пропан-бутан", value: 9 }
]
```

### Опции

Опции зависят от типа транспорта. Получить их список можно отправив GET запрос по адресу `https://developers.ria.com/auto/categories/:categoryId/options?api_key=YOUR_API_KEY`, где *categoryId* - идентификатор типа транспорта, *api_key*- Ваш ключ.

Например, список опций для легковых автомобилей ([https://developers.ria.com/auto/categories/1/options?api_key=YOUR_API_KEY](https://developers.ria.com/auto/categories/1/options?api_key=YOUR_API_KEY)) будет выглядеть примерно так:
```javascript
[
    { name: "ABD", value: 354 },
    { name: "ABS", value: 217 },
    { name: "ESP", value: 459 },
    { name: "Галогенные фары", value: 463 },
    { name: "Замок на КПП", value: 481 },
    { name: "Иммобилайзер", value: 225 },
    { name: "Пневмоподвеска", value: 442 },
    { name: "Подушка безопасности (Airbag)", value: 211 },
    { name: "Серворуль", value: 485 },
    { name: "Сигнализация", value: 303 },
    ...
]
```

## Цвета

Получить список всех цветов можно, если отправить GET запрос по адресу [https://developers.ria.com/auto/colors?api_key=YOUR_API_KEY](https://developers.ria.com/auto/colors?api_key=YOUR_API_KEY). Результат будет седующим:
```javascript
[
    { name: "Бежевый", value: 1 },
    { name: "Черный", value: 2 },
    { name: "Синий", value: 3 },
    { name: "Бронзовый", value: 4 },
    { name: "Коричневый", value: 5 },
    { name: "Золотой", value: 6 },
    { name: "Зеленый", value: 7 },
    { name: "Серый", value: 8 },
    { name: "Апельсин", value: 9 },
    { name: "Магнолии", value: 10 },
    { name: "Розовый", value: 11 },
    { name: "Фиолетовый", value: 12 },
    { name: "Красный", value: 13 },
    { name: "Серебряный", value: 14 },
    { name: "Белый", value: 15 },
    { name: "Желтый", value: 16 },
    { name: "Голубой", value: 17 },
    { name: "Вишнёвый", value: 18 },
    { name: "Сафари", value: 19 },
    { name: "Гранатовый", value: 20 },
    { name: "Асфальт", value: 21 }
]
```

### Растаможка 

Параметр растаможки может принимать только два значения: `1` - нерастаможенный и `0` - растаможенный.


### После ДТП 

Данный параметр принимает следующие значения:
`1` - объявления после ДТП
`0` - остальные объявления

### Взято в кредит 

Данный параметр может принимать следующие значения:
`1` - объявления взятые в кредит
`0` - остальные объявления

### Конфискат 

Данный параметр может принимать следующие значения:
`1` - только конфискованные объявления
`0` - только неконфискованные объявления

### Не на ходу 

Данный параметр может принимать следующие значения:
`1` - только объявления не на ходу
`0` - только объявления на ходу


### Цена 
Данный параметр может принимать значения которые Вы зададите:

`price_ot=` - цена от 

`price_do=` - цена до

### Валюта
Данный параметр может принимать следующие значения:

`1` - доллары США

`2` - евро 

`3` - гривна

### Торг
Данный параметр может принимать следующие значения:

`0` - не включать в запрос поиска

`1` - включить в запрос поиска

### Oбмен на недвижимость
Данный параметр может принимать следующие значения:

`0` - не включать в запрос поиска

`1` - включить в запрос поиска

### Oбмен на автомобиль
Данный параметр может принимать следующие значения:

`0` - не включать в запрос поиска

`1` - включить в запрос поиска

Фильтр обмена

`exchange_filter[marka_id]=0 ` - Марка автомобиля любая  

`exchange_filter[model_id]=0` - Модель автомобиля любая  

### Авто не в Украине
Данный параметр может принимать следующие значения:

`0` - по умолчанию показать все

`1` - включить в запрос поиска

`2` - не включать в запрос поиска

### Не на ходу
Данный параметр может принимать следующие значения:

`1` - отобразить

`2` - не отображать

### Продавец
Данный параметр может принимать следующие значения:

`0` - по умолчанию все

`1` - частное лицо

`2` - компания

### Пригнан из

`matched_country=` - Пригнан из

### Объем двигателя
Данный параметр может принимать значения которые Вы зададите:

`engineVolumeFrom=` - объем от 

`engineVolumeTo=`   - объем до

### Расход топлива
Данный параметр может принимать значения которые Вы зададите:

`fuelRateFrom=` - расход от

`fuelRateTo=` - рвсход до

Цикл

`fuelRatesType` может быть равен трьом значениям

`city` - городской цыкл

`combine` - шоссе

`route` - смешаный

### Мощность двигателя
Данный параметр может принимать значения которые Вы зададите:

`powerFrom=` - мощность от 

`powerTo=` - мощность до

Единица измерения мощности

`1` - лошадиные силы

`2` - кВт

### Сортировка
Данный параметр может принимать следующие значения:

`0` - по умолчанию обычная сортировка

`1` - от дешевых к дорогим

`2` - от дорогих к дешевым


### Период подачи
Данный параметр может принимать следующие значения:

`0` - по умолчанию за все время

`1` - за час

`2` - за сегодня

`3` - за три дня
 
`4` - за неделю

`5` - за месяц

`6` - за 3 месяца

`8` - за 3 часа

`9` - за 6 часов

`10` - за 2 дня

`11` - за сутки

`14` - за 12 часов

### Актуальность
Данный параметр может принимать следующие значения:

 `0` - все автомобили
 
 `1` - показывать только проданые авто
 
 `2` - неотображать проданые автомобили

### VIN код
Данный параметр может принимать следующие значения:

`0` - не включать в запрос поиска

`1` - включить в запрос поиска

### Колесная формула
Данный параметр может принимать следующие значения:

`0` - по умолчанию

`1` - 4х2

`2` - 4х4

`3` - 6х2 
 
`4` - 6х4

`5` - 6х6

`7` - 8х2

`8` - 8х4

`9` - 8х6

`10` - 8х8

`11` - 10х4

`12` - 10х8


### Количество осей
Данный параметр может принимать следующие значения:

 `0` -  по умолчанию
 
 `1` - одна ось
 
 `2` - две оси
 
 `3` - три оси
  
 `4` - четыри оси

 `5` - больше четырех осей

### Только с Фото
Данный параметр может принимать следующие значения:

`0` - не включать в запрос поиска

`1` - включить в запрос поиска
 
### Только с Видео
Данный параметр может принимать следующие значения:

`0` - не включать в запрос поиска

`1` - включить в запрос поиска

### Количество отображаемых id
Данный параметр может принимать следующие значения от `1` до `100

### Номер страницы
Данный параметр может принимать следующие значения от `1` до `100


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
