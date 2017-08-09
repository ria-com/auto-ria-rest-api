# DOM.RIA


Для получения **API_KEY** нужно зарегестрироваться на [Developers.ria.com](https://developers.ria.com/)


## Методы для работы с областями, городами, районами
### Области
Получить список областей можно отправив GET запрос по адресу [https://developers.ria.com/dom/states?api_key=YOUR_API_KEY](https://developers.ria.com/dom/states?api_key=YOUR_API_KEY).
Для получение информации на украинском языке нужно добавить параметр *lang_id=4*

Результат будет следующим:
```json
[
  {
    "lang_id": 2,
    "stateID": 1,
    "name": "Винницкая",
    "eng_name": "vinnica",
    "declension": "Винницкой области",
    "center_declension": "Винницы",
    "region_name": "Винница"
  },
  {
    "lang_id": 2,
    "stateID": 18,
    "name": "Волынская",
    "eng_name": "luck",
    "declension": "Волынской области",
    "center_declension": "Луцка",
    "region_name": "Луцк"
  },
  {
    "lang_id": 2,
    "stateID": 11,
    "name": "Днепропетровская",
    "eng_name": "dnepropetrovsk",
    "declension": "Днепропетровской области",
    "center_declension": "Днепропетровска",
    "region_name": "Днепропетровск"
  },
  {
    "lang_id": 2,
    "stateID": 13,
    "name": "Донецкая",
    "eng_name": "doneck",
    "declension": "Донецкой области",
    "center_declension": "Донецка",
    "region_name": "Донецк"
  },
  {
    "lang_id": 2,
    "stateID": 2,
    "name": "Житомирская",
    "eng_name": "jitomir",
    "declension": "Житомирской области",
    "center_declension": "Житомира",
    "region_name": "Житомир"
  },
  {
    "lang_id": 2,
    "stateID": 22,
    "name": "Закарпатская",
    "eng_name": "ujgorod",
    "declension": "Закарпатской области",
    "center_declension": "Ужгорода",
    "region_name": "Ужгород"
  },
  {
    "lang_id": 2,
    "stateID": 14,
    "name": "Запорожская",
    "eng_name": "zaporoje",
    "declension": "Запорожской области",
    "center_declension": "Запорожья",
    "region_name": "Запорожье"
  },
  {
    "lang_id": 2,
    "stateID": 15,
    "name": "Ивано-Франковская",
    "eng_name": "ivano-frankovsk",
    "declension": "Ивано-Франковской области",
    "center_declension": "Ивано-Франковска",
    "region_name": "Ивано-Франковск"
  },
  {
    "lang_id": 2,
    "stateID": 10,
    "name": "Киевская",
    "eng_name": "kiev",
    "declension": "Киевской области",
    "center_declension": "Киева",
    "region_name": "Киев"
  },
  {
    "lang_id": 2,
    "stateID": 16,
    "name": "Кировоградская",
    "eng_name": "kirovograd",
    "declension": "Кировоградской области",
    "center_declension": "Кировограда",
    "region_name": "Кировоград"
  },
  {
    "lang_id": 2,
    "stateID": 17,
    "name": "Луганская",
    "eng_name": "lugansk",
    "declension": "Луганской области",
    "center_declension": "Луганска",
    "region_name": "Луганск"
  },
  {
    "lang_id": 2,
    "stateID": 5,
    "name": "Львовская",
    "eng_name": "lvov",
    "declension": "Львовской области",
    "center_declension": "Львова",
    "region_name": "Львов"
  },
  {
    "lang_id": 2,
    "stateID": 19,
    "name": "Николаевская",
    "eng_name": "nikolaev",
    "declension": "Николаевской области",
    "center_declension": "Николаева",
    "region_name": "Николаев"
  },
  {
    "lang_id": 2,
    "stateID": 12,
    "name": "Одесская",
    "eng_name": "odessa",
    "declension": "Одесской области",
    "center_declension": "Одессы",
    "region_name": "Одесса"
  },
  {
    "lang_id": 2,
    "stateID": 20,
    "name": "Полтавская",
    "eng_name": "poltava",
    "declension": "Полтавской области",
    "center_declension": "Полтавы",
    "region_name": "Полтава"
  },
  {
    "lang_id": 2,
    "stateID": 21,
    "name": "Республика Крым",
    "eng_name": "simferopol",
    "declension": "Республики Крым",
    "center_declension": "Симферополя",
    "region_name": "Республика Крым"
  },
  {
    "lang_id": 2,
    "stateID": 9,
    "name": "Ровенская",
    "eng_name": "rovno",
    "declension": "Ровенской области",
    "center_declension": "Ровно",
    "region_name": "Ровно"
  },
  {
    "lang_id": 2,
    "stateID": 8,
    "name": "Сумская",
    "eng_name": "sumiy",
    "declension": "Сумской области",
    "center_declension": "Сум",
    "region_name": "Сумы"
  },
  {
    "lang_id": 2,
    "stateID": 3,
    "name": "Тернопольская",
    "eng_name": "ternopol",
    "declension": "Тернопольской области",
    "center_declension": "Тернополя",
    "region_name": "Тернополь"
  },
  {
    "lang_id": 2,
    "stateID": 7,
    "name": "Харьковская",
    "eng_name": "harkov",
    "declension": "Харьковской области",
    "center_declension": "Харькова",
    "region_name": "Харьков"
  },
  {
    "lang_id": 2,
    "stateID": 23,
    "name": "Херсонская",
    "eng_name": "herson",
    "declension": "Херсонской области",
    "center_declension": "Херсона",
    "region_name": "Херсон"
  },
  {
    "lang_id": 2,
    "stateID": 4,
    "name": "Хмельницкая",
    "eng_name": "hmelnickiy",
    "declension": "Хмельницкой области",
    "center_declension": "Хмельницкого",
    "region_name": "Хмельницкий"
  },
  {
    "lang_id": 2,
    "stateID": 24,
    "name": "Черкасская",
    "eng_name": "cherkassiy",
    "declension": "Черкасской области",
    "center_declension": "Черкасс",
    "region_name": "Черкассы"
  },
  {
    "lang_id": 2,
    "stateID": 6,
    "name": "Черниговская",
    "eng_name": "chernigov",
    "declension": "Черниговской области",
    "center_declension": "Чернигова",
    "region_name": "Чернигов"
  },
  {
    "lang_id": 2,
    "stateID": 25,
    "name": "Черновицкая",
    "eng_name": "chernovciy",
    "declension": "Черновицкой области",
    "center_declension": "Черновцов",
    "region_name": "Черновцы"
  }
  ```
  
  ### Города
  
  Города зависят от областей, поэтому, чтобы получить их список, необходимо послать GET запрос по адресу `https://developers.ria.com/dom/cities/:stateId?api_key=YOUR_API_KEY`, где *stateId* - идентификатор области.
  Для получение информации на украинском языке нужно добавить параметр *lang_id=4*
  
  Например, для Львовской области ([https://developers.ria.com/dom/cities/5?api_key=YOUR_API_KEY&lang_id=4](https://developers.ria.com/dom/cities/5?api_key=YOUR_API_KEY&lang_id=4) список городов будет следующим:
  
  ```json
 [
   {
     "lang_id": 4,
     "cityID": 287,
     "stateID": 5,
     "name": "Борислав",
     "eng": "borislav",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 288,
     "stateID": 5,
     "name": "Броди",
     "eng": "brodi",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 289,
     "stateID": 5,
     "name": "Буськ",
     "eng": "busk",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 290,
     "stateID": 5,
     "name": "Городок",
     "eng": "gorodok",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 291,
     "stateID": 5,
     "name": "Дрогобич",
     "eng": "drogobich",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 292,
     "stateID": 5,
     "name": "Жидачів",
     "eng": "jidachiv",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 293,
     "stateID": 5,
     "name": "Жовква",
     "eng": "jovkva",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 294,
     "stateID": 5,
     "name": "Золочев",
     "eng": "zolochev",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 295,
     "stateID": 5,
     "name": "Кам'янка-Бузька",
     "eng": "kam_yanka-buzka",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 5,
     "stateID": 5,
     "name": "Львів",
     "eng": "lviv",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 297,
     "stateID": 5,
     "name": "Миколаїв",
     "eng": "mikolayv",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 646,
     "stateID": 5,
     "name": "Моршин",
     "eng": "Morshun",
     "declension": null
   },
   {
     "lang_id": 4,
     "cityID": 298,
     "stateID": 5,
     "name": "Мостиська",
     "eng": "mostiska",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 632,
     "stateID": 5,
     "name": "Новий Розділ",
     "eng": "noviy-rozdil",
     "declension": "Новороздільский"
   },
   {
     "lang_id": 4,
     "cityID": 299,
     "stateID": 5,
     "name": "Перемишляни",
     "eng": "peremishlyani",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 300,
     "stateID": 5,
     "name": "Пустомити",
     "eng": "pustomiti",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 301,
     "stateID": 5,
     "name": "Радехів",
     "eng": "radehiv",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 302,
     "stateID": 5,
     "name": "Самбір",
     "eng": "sambir",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 303,
     "stateID": 5,
     "name": "Сколе",
     "eng": "skole",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 304,
     "stateID": 5,
     "name": "Сокаль",
     "eng": "sokal",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 614,
     "stateID": 5,
     "name": "Соснівка",
     "eng": "sosnovka",
     "declension": null
   },
   {
     "lang_id": 4,
     "cityID": 305,
     "stateID": 5,
     "name": "Старий Самбір",
     "eng": "stariyi_sambir",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 306,
     "stateID": 5,
     "name": "Стрий",
     "eng": "striyi",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 307,
     "stateID": 5,
     "name": "Трускавець",
     "eng": "truskavec",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 308,
     "stateID": 5,
     "name": "Турка",
     "eng": "turka",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 309,
     "stateID": 5,
     "name": "Червоноград",
     "eng": "chervonograd",
     "declension": ""
   },
   {
     "lang_id": 4,
     "cityID": 310,
     "stateID": 5,
     "name": "Яворів",
     "eng": "yavoriv",
     "declension": ""
   }
 ]
```  

### Районы

 Районы зависят от городов, поэтому, чтобы получить их список, необходимо послать GET запрос по адресу `https://developers.ria.com/dom/cities_districts/:city_id?api_key=YOUR_API_KEY`, где *city_id* - идентификатор города.
 Для получение информации на украинском языке нужно добавить параметр *lang_id=4*
  
Например, для города Львова ([https://developers.ria.com/dom/cities_districts/5?api_key=YOUR_API_KEY](https://developers.ria.com/dom/cities_districts/5?api_key=YOUR_API_KEY&) список районов будет следующим:
  
  ```json
  [
    [
      {
        "name": "Район",
        "value": ""
      },
      {
        "city_id": 5,
        "area_id": 15754,
        "name": "Аеропорт",
        "type": 1,
        "value": 15754
      },
      {
        "city_id": 5,
        "area_id": 15765,
        "name": "Арсен",
        "type": 1,
        "value": 15765
      },
      {
        "city_id": 5,
        "area_id": 15750,
        "name": "Білогорща",
        "type": 1,
        "value": 15750
      },
      {
        "city_id": 5,
        "area_id": 15771,
        "name": "Бондарівка",
        "type": 1,
        "value": 15771
      },
      {
        "city_id": 5,
        "area_id": 15751,
        "name": "Виговського",
        "type": 1,
        "value": 15751
      },
      {
        "city_id": 5,
        "area_id": 15763,
        "name": "Винники",
        "type": 1,
        "value": 15763
      },
      {
        "city_id": 5,
        "area_id": 15087,
        "name": "Галицький",
        "type": 1,
        "value": 15087
      },
      {
        "city_id": 5,
        "area_id": 15777,
        "name": "Голоско",
        "type": 1,
        "value": 15777
      },
      {
        "city_id": 5,
        "area_id": 15088,
        "name": "Залізничний",
        "type": 1,
        "value": 15088
      },
      {
        "city_id": 5,
        "area_id": 15778,
        "name": "Замарстинів",
        "type": 1,
        "value": 15778
      },
      {
        "city_id": 5,
        "area_id": 15779,
        "name": "Збоїща",
        "type": 1,
        "value": 15779
      },
      {
        "city_id": 5,
        "area_id": 15760,
        "name": "Знесення",
        "type": 1,
        "value": 15760
      },
      
      {
        "city_id": 5,
        "area_id": 15767,
        "name": "Новий Львів",
        "type": 1,
        "value": 15767
      },
      {
        "city_id": 5,
        "area_id": 15773,
        "name": "Новий Світ",
        "type": 1,
        "value": 15773
      },
      {
        "city_id": 5,
        "area_id": 15768,
        "name": "Пасіки",
        "type": 1,
        "value": 15768
      },
      {
        "city_id": 5,
        "area_id": 15772,
        "name": "Персеньківка",
        "type": 1,
        "value": 15772
      },
      {
        "city_id": 5,
        "area_id": 15769,
        "name": "Пироговка",
        "type": 1,
        "value": 15769
      },
      
      .......................
      
      
      {
        "city_id": 5,
        "area_id": 15775,
        "name": "Ринок Південний",
        "type": 1,
        "value": 15775
      },
      {
        "city_id": 5,
        "area_id": 15748,
        "name": "Рясне",
        "type": 1,
        "value": 15748
      },
      {
        "city_id": 5,
        "area_id": 15766,
        "name": "Санта Барбара",
        "type": 1,
        "value": 15766
      },
      {
        "city_id": 5,
        "area_id": 15753,
        "name": "Сигнівка",
        "type": 1,
        "value": 15753
      },
      {
        "city_id": 5,
        "area_id": 15090,
        "name": "Сихівський",
        "type": 1,
        "value": 15090
      },
      {
        "city_id": 5,
        "area_id": 15752,
        "name": "Скнилів",
        "type": 1,
        "value": 15752
      },
      {
        "city_id": 5,
        "area_id": 15747,
        "name": "Снопківська",
        "type": 1,
        "value": 15747
      },
      {
        "city_id": 5,
        "area_id": 15764,
        "name": "ТЦ Іскра",
        "type": 1,
        "value": 15764
      },
      {
        "city_id": 5,
        "area_id": 15091,
        "name": "Франківський",
        "type": 1,
        "value": 15091
      },
      {
        "city_id": 5,
        "area_id": 15745,
        "name": "Цитадель",
        "type": 1,
        "value": 15745
      },
      {
        "city_id": 5,
        "area_id": 15092,
        "name": "Шевченківський",
        "type": 1,
        "value": 15092
      }
    ],
    [
      {
        "name": "Пригород",
        "value": ""
      },
      {
        "city_id": 5,
        "area_id": 7494,
        "name": "Брюховичі",
        "type": 2,
        "value": 7494
      },
      {
        "city_id": 5,
        "area_id": 15742,
        "name": "Зимна Вода",
        "type": 2,
        "value": 15742
      },
      {
        "city_id": 5,
        "area_id": 15743,
        "name": "Малечковичі",
        "type": 2,
        "value": 15743
      },
      {
        "city_id": 5,
        "area_id": 15741,
        "name": "Сокільники",
        "type": 2,
        "value": 15741
      }
    ],
    [
      {
        "name": "Село",
        "value": ""
      },
      {
        "city_id": 5,
        "area_id": 7495,
        "name": "Винники",
        "type": 3,
        "value": 7495
      },
      {
        "city_id": 5,
        "area_id": 17513,
        "name": "Липники",
        "type": 3,
        "value": 17513
      },
      {
        "city_id": 5,
        "area_id": 7497,
        "name": "Рудне",
        "type": 3,
        "value": 7497
      }
    ]
  ]
  
  
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