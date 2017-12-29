# DOM.RIA

Для получения **API_KEY** нужно зарегестрироваться на [Developers.ria.com](https://developers.ria.com/)

## Параметры для работы с DOM.RIA API

### Продажа квартир/комнат

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|   `Number`      |
|Тип недвижимости |realty_type |    `Number`        |
|Тип операции | operation_type|     `Number`       |
|Область | state_id| `Number` |
|Город | city_id| `Number[]` |
|Район | district_id|`Number[]`  |
|Тип стен| characteristic[118] |`Number[]`  |
|Количество комнат |characteristic[209][from] - characteristic[209][to] | `Number[]` |
|Общая площадь |characteristic[214][from] - characteristic[214][to] |`Number[]`  |
|Жилая площадь |characteristic[216][from] - characteristic[216][to] |`Number[]`  |
|Кухня |characteristic[218][from] - characteristic[218][to] |`Number[]`  |
|Этаж |characteristic[227][from] - characteristic[227][to] | `Number[]` |
|Этажность |characteristic[228][from] - characteristic[228][to] | `Number[]` |
|Кухня студия |characteristic[1501] | `Number` |
|Пентхаус |characteristic[1504] |`Number` |
|Многоуровневая|characteristic[1502] |`Number` |
|С мансардой |characteristic[1503] |`Number` |
|Год постройки |characteristic[443] |`Number` |
|Коммунальные платежи в зимний период |characteristic[1607][from] - characteristic[1607][to] |`Number[]` |
|Коммунальные платежи в летний период |characteristic[1608][from] - characteristic[1608][to] | `Number[]`|
|Цена |characteristic[234][from] - characteristic[234][to] | `Number[]`|
|Цена за (объект / квадратный метр) |characteristic[247] |`Number` |
|Цена договорная |characteristic[1011] |`Number` |
|Стартовая цена |characteristic[1464] |`Number` |
|Тип валюты |characteristic[246] |`Number` |
|Возможен обмен |characteristic[265] | `Number`|
|Возможен торг |characteristic[273] | `Number`|
|Тип предложения |characteristic[1437] |`Number` |
|Возможна расстрочка/кредит |characteristic[274] | `Number`|
|Только с картой |with_map |`Number` |
|Только с видео | with_video |`Number` |
|Только с фото |with_photo |`Number` |
|Только с фото (более 3 фото)| photos_count_from| `Number`|
|Только ТОП| urgent_only|`Number` |
|Залоговое имущество | banks_only|`Number` |
|Вторичное жилье |secondary |`Number` |
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to |`Number` |
|Страница|page | |

### Аренда квартир/комнат

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|    `Number`    |
|Тип недвижимости |realty_type |    `Number`       |
|Тип операции | operation_type|    `Number`       |
|Область | state_id|`Number` |
|Город | city_id|`Number[]` |
|Район | district_id|`Number[]` |
|Тип стен| characteristic[118] | `Number[]`|
|Количество комнат |characteristic[209][from] - characteristic[209][to] |`Number[]` |
|Общая площадь |characteristic[214][from] - characteristic[214][to] |`Number[]` |
|Жилая площадь |characteristic[216][from] - characteristic[216][to] |`Number[]` |
|Кухня |characteristic[218][from] - characteristic[218][to] |`Number[]` |
|Этаж |characteristic[227][from] - characteristic[227][to] | `Number[]`|
|Этажность |characteristic[228][from] - characteristic[228][to] |`Number[]` |
|С джакузи| characteristic[1481]|`Number` |
|С отоплением| characteristic[1478]|`Number` |
|С мебелью |characteristic[1480] |`Number` |
|С ремонтом |characteristic[1479] | `Number`|
|Дополнительные платежи |characteristic[254] |`Number` |
|С подсилением |characteristic[1500] |`Number` |
|Совместная аренда |characteristic[1596] |`Number` |
|Коммунальные платежи в зимний период |characteristic[1609][from] - characteristic[1609][to] | `Number[]`|
|Коммунальные платежи в летний период |characteristic[1610][from] - characteristic[1610][to] | `Number[]`|
|Цена/месяц |characteristic[235][from] - characteristic[235][to] | `Number[]`|
|Цена договорная |characteristic[1011] | `Number`|
|Детализация **(Аренда посуточно)** |characteristic[1399] |`Number` |
|Кухня студия **(Аренда посуточно)**|characteristic[1501] |`Number` |
|На выходные **(Аренда посуточно)** |characteristic[1477] | `Number`|
|На празники **(Аренда посуточно)** |characteristic[1498] | `Number`|
|На новый год **(Аренда посуточно)** |characteristic[1499] |`Number` |
|Цена/сутки  **(Аренда посуточно)** |characteristic[237][from] - characteristic[237][to] | `Number[]`|
|Цена/час  **(Аренда посуточно)** |characteristic[238][from] - characteristic[238][to] |`Number[]` |
|Цена/неделю |characteristic[279][from] - characteristic[279][to] |`Number[]` |
|Тип валюты |characteristic[246] | `Number`|
|Тип предложения |characteristic[1437] | `Number`|
|Только с картой |with_map |`Number` |
|Только с видео | with_video | `Number`|
|Только с фото |with_photo | `Number`|
|Только с фото (более 3 фото)| photos_count_from|`Number` |
|Только ТОП| urgent_only|`Number` |
|Залоговое имущество | banks_only| `Number`|
|Вторичное жилье |secondary | `Number`|
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to |`Number` |
|Страница|page |`Number` |


### Продажа домов

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|     `Number`   |
|Тип недвижимости |realty_type |    `Number`       |
|Тип операции | operation_type|    `Number`       |
|Область | state_id| `Number`|
|Город | city_id|`Number[]` |
|Район | district_id| `Number[]`|
|Тип стен | characteristic[149]|`Number` |
|Количество комнат |characteristic[209][from] - characteristic[209][to] | `Number[]`|
|Общая площадь |characteristic[215][from] - characteristic[215][to] |`Number[]` |
|Жилая площадь |characteristic[216][from] - characteristic[216][to] |`Number[]` |
|Кухня |characteristic[218][from] - characteristic[218][to] | `Number[]`|
|Участок |characteristic[219][from] - characteristic[219][to] | `Number[]`|
|Единица измерения площади участка |characteristic[226] | `Number[]`|
|C беседкой   |characteristic[1492] |`Number` |
|С верандой   |characteristic[1491] |`Number` |
|С подвалом  |characteristic[1490] | `Number`|
|С балконом |characteristic[1489] |`Number` |
|С камином |characteristic[1488] |`Number` |
|С садом  |characteristic[1487] | `Number`|
|С баней/сауной |characteristic[1486] |`Number` |
|С террасой |characteristic[1485] |`Number` |
|С гаражом  |characteristic[1484] | `Number`|
|С участком  |characteristic[1505] |`Number` |
|С мансардою   |characteristic[1482] |`Number` |
|С мебелью |characteristic[1480] | `Number`|
|С ремонтом |characteristic[1479] |`Number` |
|С отоплением   |characteristic[1478] | `Number`|
|Мансардный этаж |characteristic[230] | `Number`|
|Подвальный / цокольный этаж |characteristic[231] | `Number`|
|У озера **Дача** |characteristic[1494] |`Number` |
|У реки **Дача** |characteristic[1493] | `Number`|
|Жилых этажей |characteristic[229][from] - characteristic[229][to] | `Number[]`|
|Год постройки |characteristic[443] | `Number`|
|Цена |characteristic[234][from] -characteristic[234][to] |`Number[]` |
|Цена договорная |characteristic[1011]|`Number` |
|Стартовая цена |characteristic[1464] |`Number` |
|Тип валюты |characteristic[242] | `Number`|
|Возможен обмен |characteristic[265] | `Number`|
|Возможен торг | characteristic[273]| `Number`|
|Тип предложения |characteristic[1437] | `Number`|
|Возможна расстрочка/кредит |characteristic[274] |`Number` |
|Только с картой |with_map |`Number` |
|Только с видео | with_video | `Number`|
|Только с фото |with_photo |`Number` |
|Только с фото (более 3 фото)| photos_count_from|`Number` |
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only|`Number` |
|Вторичное жилье |secondary | `Number`|
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my|`Number` |
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to |`Number` |
|Страница|page |`Number` |


### Аренда домов

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|      `Number`  |
|Тип недвижимости |realty_type |    `Number`       |
|Тип операции | operation_type|  `Number`         |
|Область | state_id| `Number`|
|Город | city_id| `Number[]`|
|Район | district_id|`Number[]` |
|Тип стен | characteristic[149]| `Number`|
|Количество комнат |characteristic[209][from] - characteristic[209][to] |`Number[]` |
|Общая площадь |characteristic[215][from] - characteristic[215][to] |`Number[]` |
|Жилая площадь |characteristic[216][from] - characteristic[216][to] |`Number[]` |
|С балконом |characteristic[1489] |`Number` |
|С камином |characteristic[1488] | `Number`|
|С бассейном  |characteristic[1483] | `Number`|
|С баней/сауной |characteristic[1486] |`Number` |
|С гаражом  |characteristic[1484] |`Number` |
|С мебелью |characteristic[1480] | `Number`|
|С ремонтом |characteristic[1479] | `Number`|
|Мансардный этаж |characteristic[230] | `Number`|
|Подвальный / цокольный этаж |characteristic[231] | `Number`|
|Цена/месяц |characteristic[235][from] - characteristic[235][to] |`Number[]` |
|Цена договорная |characteristic[1011] |`Number` |
|Дополнительные платежи |characteristic[254] | `Number`|
|Детализация **(Аренда посуточно)** |characteristic[1399] |`Number` |
|Спальных мест от **(Аренда посуточно)** |characteristic[212][from] - characteristic[212][to] |`Number[]` |
|На день рождения **(Аренда посуточно)** |characteristic[1595] | `Number`|
|Цена/сутки  **(Аренда посуточно)** |characteristic[237][from] - characteristic[237][to] |`Number[]` |
|Цена/час  **(Аренда посуточно)** |characteristic[238][from] - characteristic[238][to] |`Number[]` |
|Цена/неделю |characteristic[279][from] - characteristic[279][to] |`Number[]` |
|Тип валюты |characteristic[246] | `Number`|
|Тип предложения |characteristic[1437] | `Number`|
|Только с картой |with_map |`Number` |
|Только с видео | with_video | `Number`|
|Только с фото |with_photo | `Number`|
|Только с фото (более 3 фото)| photos_count_from|`Number` |
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only|`Number` |
|Вторичное жилье |secondary | `Number`|
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to |`Number` |
|Страница|page |`Number` |


### Продажа офисов

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|    `Number`    |
|Тип недвижимости |realty_type |      `Number`     |
|Тип операции | operation_type|    `Number`       |
|Область | state_id|`Number` |
|Город | city_id| `Number[]`|
|Район | district_id|`Number[]` |
|Количество помещений |characteristic[210][from] - characteristic[210][to] | `Number[]`|
|Тип объекта для Офисов |characteristic[162] | `Number`|
|Общая |characteristic[214][from] - characteristic[214][to] | `Number[]`|
|Полезная |characteristic[217][from] - characteristic[217][to] | `Number[]`|
|Этаж |characteristic[227][from] - characteristic[227][to] | `Number[]`|
|Этажность |characteristic[228][from] - characteristic[228][to] | `Number[]`|
|Участок |characteristic[219][from] - characteristic[219][to] |`Number[]` |
|Цена за (объект/кв.м.) |characteristic[247] |`Number` |
|Единица измерения площади участка |characteristic[226] |`Number`|
|Мансардный этаж |characteristic[230] | `Number`|
|Подвальный / цокольный этаж |characteristic[231] | `Number`|
|Цена |characteristic[234][from] - characteristic[234][to] | `Number[]`|
|Цена договорная |characteristic[1011] | `Number`|
|Стартовая цена |characteristic[1464] | `Number`|
|Возможен торг |characteristic[273] | `Number`|
|Возможна расстрочка/кредит |characteristic[274] | `Number`|
|Возможен обмен |characteristic[265] |`Number` |
|Тип валюты |characteristic[242] | `Number`|
|Тип предложения |characteristic[1437] | `Number`|
|Возможна расстрочка/кредит |characteristic[274] | `Number`|
|Только с картой |with_map | `Number`|
|Только с видео | with_video | `Number`|
|Только с фото |with_photo |`Number` |
|Только с фото (более 3 фото)| photos_count_from| `Number`|
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only| `Number`|
|Вторичное жилье |secondary |`Number` |
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies | `Number`|
|Дата подачи |date_from - date_to |`Number` |
|Страница|page |`Number` |


### Аренда офисов

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|       `Number` |
|Тип недвижимости |realty_type |    `Number`       |
|Тип операции | operation_type|     `Number`      |
|Область | state_id|`Number` |
|Город | city_id|`Number[]` |
|Район | district_id| `Number[]`|
|Количество помещений |characteristic[210][from] - characteristic[210][to] | `Number[]`|
|Тип объекта для Офисов |characteristic[155] | `Number`|
|Общая |characteristic[214][from] - characteristic[214][to] | `Number[]`|
|Полезная |characteristic[217][from] - characteristic[217][to] | `Number[]`|
|Этаж |characteristic[227][from] - characteristic[227][to] |`Number[]` |
|Этажность |characteristic[228][from] - characteristic[228][to] | `Number[]`|
|Цена/месяц |characteristic[235][from] - characteristic[235][to] | `Number[]`|
|Цена договорная |characteristic[1011] | `Number`|
|Дополнительные платежи |characteristic[254] |`Number` |
|Возможен торг |characteristic[273] | `Number`|
|Тип валюты |characteristic[242] | `Number`|
|Цена за (объект/кв.м.) |characteristic[247] |`Number` |
|Тип предложения |characteristic[1437] |`Number` |
|Возможна расстрочка/кредит |characteristic[274] |`Number` |
|Только с картой |with_map |`Number` |
|Только с видео | with_video | `Number`|
|Только с фото |with_photo | `Number`|
|Только с фото (более 3 фото)| photos_count_from| `Number`|
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only| `Number`|
|Вторичное жилье |secondary |`Number` |
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies | `Number`|
|Дата подачи |date_from - date_to | `Number`|
|Страница|page | `Number`|

### Продажа/аренда коммерческой недвижимости

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|  `Number`      |
|Тип недвижимости |realty_type |     `Number`      |
|Тип операции | operation_type|   `Number`        |
|Область | state_id|`Number` |
|Город | city_id|`Number[]` |
|Район | district_id| `Number[]`|
|Количество помещений |characteristic[210][from] - characteristic[210][to] |`Number[]` |
|Тип объекта-торговые площади |characteristic[169] | `Number`|
|Общая |characteristic[214][from] - characteristic[214][to] | `Number[]`|
|Полезная |characteristic[217][from] - characteristic[217][to] | `Number[]`|
|Этаж |characteristic[227][from] - characteristic[227][to] |`Number[]` |
|Этажность |characteristic[228][from] - characteristic[228][to] | `Number[]`|
|Участок |characteristic[219][from] - characteristic[219][to] |`Number[]` |
|Единица измерения площади участка |characteristic[226] | `Number`|
|Сфера **Готовый бизнес** |characteristic[199] | `Number`|
|Тип объекта-складские помещени |characteristic[159] | `Number`|
|Тип объекта-производственные помещения |characteristic[162] |`Number` |
|Действующий бизнес |characteristic[1438] | `Number`|
|Цена |characteristic[235][from] - characteristic[235][to] |`Number[]` |
|Цена/месяц **Аренда**|characteristic[235][from] - characteristic[235][to] |`Number[]` |
|Дополнительные платежи **Аренда** |characteristic[254] |`Number` |
|Цена договорная |characteristic[1011] |`Number` |
|Стартовая цена |characteristic[1464] |`Number` |
|Тип валюты |characteristic[242] |`Number` |
|Возможен обмен |characteristic[265] | `Number`|
|Возможен торг |characteristic[273] | `Number`|
|Возможна расстрочка/кредит |characteristic[274] | `Number`|
|Цена за (объект / квадратный метр) |characteristic[247] |`Number` |
|Тип предложения |characteristic[1437] |`Number` |
|Только с картой |with_map | `Number`|
|Только с видео | with_video | `Number`|
|Только с фото |with_photo | `Number`|
|Только с фото (более 3 фото)| photos_count_from| `Number`|
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only| `Number`|
|Вторичное жилье |secondary | `Number`|
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to | `Number`|
|Страница|page |`Number` |

### Продажа/аренда земельных участков

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|   `Number`     |
|Тип недвижимости |realty_type |     `Number`      |
|Тип операции | operation_type|    `Number`       |
|Область | state_id| `Number`|
|Город | city_id| `Number[]`|
|Район | district_id|`Number[]` |
|Площадь примерно от |characteristic[1424][from] - characteristic[1424][to] |`Number[]` |
|Площадь примерно до |characteristic[1465][from] - characteristic[1465][to] | `Number[]`|
|Единица измерения площади участка |characteristic[226] | `Number`|
|В коттеджном городке |characteristic[1604] | `Number`|
|Свет |characteristic[1601] |`Number` |
|Вода |characteristic[1602] | `Number`|
|Газ |characteristic[1600] | `Number`|
|Канализация |characteristic[1603] |`Number` |
|Цена |characteristic[234][from] - characteristic[234][to] |`Number[]` |
|Тип цены|characteristic[251] | `Number`|
|Цена договорная |characteristic[1011] |`Number` |
|Стартовая цена |characteristic[1464] | `Number`|
|Тип валюты |characteristic[242] |`Number` |
|Возможен обмен |characteristic[265] | `Number`|
|Возможен торг |characteristic[273] |`Number` |
|Возможна расстрочка/кредит |characteristic[274] |`Number` |
|Цена/год **Аренда** |characteristic[236][from] - characteristic[236][to] |`Number[]` |
|Предоплата **Аренда** |characteristic[1362][from] - characteristic[1362][to] | `Number[]`|
|Тип предложения |characteristic[1437] |`Number` |
|Только с картой |with_map | `Number`|
|Только с видео | with_video | `Number`|
|Только с фото |with_photo |`Number` |
|Только с фото (более 3 фото)| photos_count_from| `Number`|
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only| `Number`|
|Вторичное жилье |secondary | `Number`|
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to | `Number`|
|Страница|page |`Number` |

### Продажа/аренда гаражей

|  Название           | Параметр в строке запроса | Тип данных   |
|:--------------------|:--------------------------|:------------:|
|Тип объекта | category|   `Number`     |
|Тип недвижимости |realty_type |    `Number`       |
|Тип операции | operation_type|    `Number`       |
|Область | state_id| `Number`|
|Город | city_id| `Number[]`|
|Район | district_id|`Number[]` |
|Машиномест |characteristic[211][from] - characteristic[211][to] | `Number[]`|
|Общая |characteristic[214][from] - characteristic[214][to] | `Number[]`|
|Назначение |characteristic[175] | `Number`|
|Цена |characteristic[234][from] - characteristic[234][to] |`Number[]` |
|Цена |characteristic[235][from] - characteristic[235][to] | `Number[]`|
|Цена договорная |characteristic[1011] | `Number`|
|Стартовая цена |characteristic[1464] | `Number`|
|Тип валюты |characteristic[242] |`Number` |
|Возможен обмен |characteristic[265] | `Number`|
|Возможен торг |characteristic[273] |`Number` |
|Возможна расстрочка/кредит |characteristic[274] | `Number`|
|Тип предложения |characteristic[1437] | `Number`|
|Только с картой |with_map | `Number`|
|Только с видео | with_video | `Number`|
|Только с фото |with_photo |`Number` |
|Только с фото (более 3 фото)| photos_count_from|`Number` |
|Только ТОП| urgent_only| `Number`|
|Залоговое имущество | banks_only|`Number` |
|Вторичное жилье |secondary | `Number`|
|Первичное жилье | newbuildings| `Number`|
|Не показывать мои объявления | exclude_my| `Number`|
|Не показывать объявления от агентств|exclude_agencies |`Number` |
|Дата подачи |date_from - date_to |`Number` |
|Страница|page |`Number` |


## Тип объекта

Данный параметр может принимать следующие значения:

`1` Квартиры

`4` Дома

`13` Офисы

`10` Коммерческая

`24` Участки

`30` Гаражи 

## Тип недвижимости

Тип недвижимости зависит от типа объекта. Следовательно, для **'Квартиры'** тип недвижимости будет следующим:

`2` Квартира

`3` Комнаты

**Для 'Дома':**

`5` Дом

`6` Часть

`7` Дачи

**Для офисов:**

`11` Офисные помещения

`12` Офисные здания

**Для коммерческой недвижимости:**

`14` Площади

`15` Склады

`16` Производство

`17` Рестораны

`18` Объект

`19` Отель

`20` Пансионаты

`21` Помещения свободного назначения

`22` Бизнес

**Для участков:**

`25` Под застройку

`26` Коммерческие

`27` Сельскохозяйственные

`28` Рекреационные

`29` Природные

**Для гаражей:**

`31` Бокс

`32` Паркинг

`33` Кооператив

`34` Гараж

`35` Стоянка



## Тип операции

`0` Любая операция

`1` Продажа

`3` Долгострочная аренда

`4` Посуточная аренда


## Список характеристик недвижимости

Получить список областей можно отправив GET запрос по адресу [https://developers.ria.com/dom/options?category=id&realty_type=id&operation_type=id&api_key=YOUR_API_KEY](https://developers.ria.com/dom/options?category=id&realty_type=id&operation_type=id&api_key=YOUR_API_KEY).
, где 

- *category* - тип объекта

- *realty_type* - тип недвижимости

- *operation_type* - тип операции

или `curl -X GET "https://developers.ria.com/dom/options?category=id&realty_type=id&operation_type=id&api_key=YOUR_API_KEY" -H "accept: application/json"`

Для получение информации на украинском языке нужно добавить параметр *lang_id=4*

Полное описание сервиса "Список характеристик недвижимости" описанный с помощью стандарта DeFacto swagger 2.0 [здесь](http://swagger.ria.com/ui/?api=dom/options)

**Пример**

Допусти Вам нужно получить список характеристик объекта 'Дома', а тип недвижимости - 'Дачи', тип операции - 'Продажа'

Данный запрос будет выглядеть так:

https://developers.ria.com/dom/options?category=4&realty_type=7&operation_type=1&api_key=YOUR_API_KEY

или `curl -X GET "https://developers.ria.com/dom/options?category=4&realty_type=7&operation_type=1&api_key=YOUR_API_KEY" -H "accept: application/json"`

Результат будет следующим:
```json
[
  {
    "group_name": "комнаты",
    "group_prio": 150,
    "items": [
      {
        "characteristic_id": 209,
        "label": "комнат",
        "label_uk": "кімнат",
        "type_on_add": "text",
        "type_on_search": "text",
        "data_type": "int",
        "required": 1,
        "characteristic_category": "main",
        "prio": 150,
        "name": "Комнат",
        "group_name": "комнаты",
        "group_name_uk": "кімнати",
        "field_name": "rooms_count",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic",
        "group_prio": 0
      }
    ]
  },
  {
    "group_name": "Тип стен",
    "group_prio": 100,
    "items": [
      {
        "characteristic_id": 149,
        "label": "тип стен",
        "label_uk": "тип стін",
        "type_on_add": "select",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 1,
        "characteristic_category": "main",
        "prio": 100,
        "name": "тип стен для дома",
        "group_name": "Тип стен",
        "group_name_uk": "Тип стін",
        "children": {
          "129": {
            "characteristic_id": "129",
            "name": "кирпич",
            "name_uk": "цегла",
            "prio": "200"
          },
          "130": {
            "characteristic_id": "130",
            "name": "кирпич силикатный",
            "name_uk": "цегла силікатна",
            "prio": "190"
          },
          "131": {
            "characteristic_id": "131",
            "name": "кирпич саманный",
            "name_uk": "цегла саманна",
            "prio": "180"
          },
          "132": {
            "characteristic_id": "132",
            "name": "дерево и кирпич",
            "name_uk": "дерево та цегла",
            "prio": "170"
          },
          "133": {
            "characteristic_id": "133",
            "name": "панель",
            "name_uk": "панель",
            "prio": "160"
          },
          "134": {
            "characteristic_id": "134",
            "name": "пеноблок",
            "name_uk": "пеноблок",
            "prio": "150"
          },
          "135": {
            "characteristic_id": "135",
            "name": "керамзитобетон",
            "name_uk": "керамзітобетон",
            "prio": "140"
          },
          "136": {
            "characteristic_id": "136",
            "name": "монолит",
            "name_uk": "моноліт",
            "prio": "130"
          },
          "138": {
            "characteristic_id": "138",
            "name": "сруб",
            "name_uk": "зруб",
            "prio": "110"
          },
          "139": {
            "characteristic_id": "139",
            "name": "брус",
            "name_uk": "брус",
            "prio": "100"
          },
          "140": {
            "characteristic_id": "140",
            "name": "каркасно-щитовой",
            "name_uk": "каркасно-щитовий",
            "prio": "90"
          },
          "141": {
            "characteristic_id": "141",
            "name": "глинобитный",
            "name_uk": "глинобитний",
            "prio": "80"
          },
          "142": {
            "characteristic_id": "142",
            "name": "пенобетон",
            "name_uk": "пінобетон",
            "prio": "70"
          },
          "143": {
            "characteristic_id": "143",
            "name": "газобетон",
            "name_uk": "газобетон",
            "prio": "60"
          },
          "144": {
            "characteristic_id": "144",
            "name": "сендвич-панели",
            "name_uk": "сендвіч-панелі",
            "prio": "50"
          },
          "145": {
            "characteristic_id": "145",
            "name": "метал",
            "name_uk": "метал",
            "prio": "40"
          },
          "146": {
            "characteristic_id": "146",
            "name": "поротерм",
            "name_uk": "поротерм",
            "prio": "30"
          },
          "147": {
            "characteristic_id": "147",
            "name": "ракушечник (ракушняк)",
            "name_uk": "ракушняк",
            "prio": "20"
          },
          "148": {
            "characteristic_id": "148",
            "name": "инкерманский камень",
            "name_uk": "інкерманський камінь",
            "prio": "10"
          },
          "1433": {
            "characteristic_id": "1433",
            "name": "шлакобетон",
            "name_uk": "шлакобетон",
            "prio": "65"
          },
          "1441": {
            "characteristic_id": "1441",
            "name": "шлакоблок",
            "name_uk": "шлакоблок",
            "prio": "55"
          },
          "1442": {
            "characteristic_id": "1442",
            "name": "наливной",
            "name_uk": "наливний",
            "prio": "5"
          },
          "1444": {
            "characteristic_id": "1444",
            "name": "бутовый камень",
            "name_uk": "бутовий камінь",
            "prio": "4"
          },
          "1445": {
            "characteristic_id": "1445",
            "name": "мергель",
            "name_uk": "мергель",
            "prio": "3"
          },
          "1447": {
            "characteristic_id": "1447",
            "name": "крупноблочный известняк",
            "name_uk": "великоблочний вапняк",
            "prio": "2"
          },
          "1463": {
            "characteristic_id": "1463",
            "name": "термоблок",
            "name_uk": "термоблок",
            "prio": "1"
          },
          "1597": {
            "characteristic_id": "1597",
            "name": "сип панель ",
            "name_uk": "сіп панель",
            "prio": "56"
          },
          "1598": {
            "characteristic_id": "1598",
            "name": "контейнер ",
            "name_uk": "контейнер",
            "prio": "7"
          }
        },
        "field_name": "wall_type",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic",
        "group_prio": 0
      }
    ]
  },
  {
    "group_name": "площадь помещений",
    "group_prio": 90,
    "items": [
      {
        "characteristic_id": 215,
        "label": "общая пл.",
        "label_uk": "загальна пл.",
        "type_on_add": "text",
        "type_on_search": "text",
        "data_type": "float",
        "required": 1,
        "sufix": "м.кв.",
        "characteristic_category": "main",
        "prio": 4,
        "name": "площадь дома",
        "group_name": "площадь помещений",
        "group_name_uk": "площа приміщень",
        "group_prio": 90,
        "field_name": "total_square_meters",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 216,
        "label": "жилая",
        "label_uk": "житлова",
        "type_on_add": "text",
        "type_on_search": "text",
        "data_type": "float",
        "required": 0,
        "sufix": "кв. м",
        "characteristic_category": "main",
        "prio": 3,
        "name": "жилая площадь",
        "group_name": "площадь помещений",
        "group_name_uk": "площа приміщень",
        "group_prio": 90,
        "field_name": "living_square_meters",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 218,
        "label": "кухня",
        "label_uk": "кухня",
        "type_on_add": "text",
        "type_on_search": "text",
        "data_type": "float",
        "required": 0,
        "sufix": "кв. м",
        "characteristic_category": "main",
        "prio": 2,
        "name": "кухня",
        "group_name": "площадь помещений",
        "group_name_uk": "площа приміщень",
        "group_prio": 90,
        "field_name": "kitchen_square_meters",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      }
    ]
  },
  {
    "group_name": "площадь участка",
    "group_prio": 83,
    "items": [
      {
        "characteristic_id": 219,
        "label": "участок",
        "label_uk": "ділянка",
        "type_on_add": "text",
        "type_on_search": "text",
        "data_type": "float",
        "required": 0,
        "characteristic_category": "main",
        "prio": 10,
        "name": "площадь участка",
        "group_name": "площадь участка",
        "group_name_uk": "площа ділянки",
        "group_prio": 85,
        "field_name": "ares_count",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 226,
        "label": "единица измерения",
        "label_uk": "одиниця виміру",
        "type_on_add": "select",
        "type_on_search": "select",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 2,
        "name": "единица измерения площади участка",
        "group_name": "площадь участка",
        "group_name_uk": "площа ділянки",
        "group_prio": 83,
        "children": {
          "223": {
            "characteristic_id": "223",
            "name": "сотка",
            "name_uk": "сотка",
            "prio": "3"
          },
          "224": {
            "characteristic_id": "224",
            "name": "Га (гектар)",
            "name_uk": "Га (гектар)",
            "prio": "2"
          },
          "225": {
            "characteristic_id": "225",
            "name": "кв. м",
            "name_uk": "кв. м",
            "prio": "1"
          }
        },
        "field_name": "lot_unit",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      }
    ]
  },
  {
    "group_name": "этаж",
    "group_prio": 75,
    "items": [
      {
        "characteristic_id": 1494,
        "label": "у озера",
        "label_uk": "біля озера",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 4,
        "name": "у озера",
        "group_name": "этаж",
        "group_name_uk": "поверх",
        "group_prio": 75,
        "display_label_search": 1,
        "display_label_add": 1,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 1493,
        "label": "у реки",
        "label_uk": "біля річки",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 3,
        "name": "у реки",
        "group_name": "этаж",
        "group_name_uk": "поверх",
        "group_prio": 75,
        "display_label_search": 1,
        "display_label_add": 1,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 230,
        "label": "мансардный этаж",
        "label_uk": "мансардний поверх",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 2,
        "name": "мансардный этаж",
        "group_name": "этаж",
        "group_name_uk": "поверх",
        "group_prio": 75,
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 231,
        "label": "подвальный / цокольный этаж",
        "label_uk": "підвальний / цокольний поверх",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 1,
        "name": "подвальный / цокольный этаж",
        "group_name": "этаж",
        "group_name_uk": "поверх",
        "group_prio": 75,
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      }
    ]
  },
  {
    "group_name": "характеристика здания",
    "group_prio": 70,
    "items": [
      {
        "characteristic_id": 443,
        "label": "год постройки",
        "label_uk": "рік побудови",
        "type_on_add": "select",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "default_value": "не указано",
        "characteristic_category": "main",
        "prio": 160,
        "name": "год постройки",
        "group_name": "характеристика здания",
        "group_name_uk": "характеристика будівлі",
        "group_prio": 70,
        "children": {
          "421": {
            "characteristic_id": "421",
            "name": "2015, IV кв.",
            "name_uk": "2015, IV кв.",
            "prio": "25"
          },
          "422": {
            "characteristic_id": "422",
            "name": "2013",
            "name_uk": "2013",
            "prio": "20"
          },
          "423": {
            "characteristic_id": "423",
            "name": "2012",
            "name_uk": "2012",
            "prio": "19"
          },
          "424": {
            "characteristic_id": "424",
            "name": "2011 ",
            "name_uk": "2011",
            "prio": "18"
          },
          "425": {
            "characteristic_id": "425",
            "name": "2010",
            "name_uk": "2010",
            "prio": "17"
          },
          "426": {
            "characteristic_id": "426",
            "name": "2009",
            "name_uk": "2009",
            "prio": "16"
          },
          "427": {
            "characteristic_id": "427",
            "name": "2008",
            "name_uk": "2008",
            "prio": "15"
          },
          "428": {
            "characteristic_id": "428",
            "name": "2007",
            "name_uk": "2007",
            "prio": "14"
          },
          "429": {
            "characteristic_id": "429",
            "name": "2006",
            "name_uk": "2006",
            "prio": "13"
          },
          "434": {
            "characteristic_id": "434",
            "name": "2001-2005",
            "name_uk": "2001-2005",
            "prio": "8"
          },
          "435": {
            "characteristic_id": "435",
            "name": "1990-2000",
            "name_uk": "1990-2000",
            "prio": "7"
          },
          "436": {
            "characteristic_id": "436",
            "name": "1980-1989",
            "name_uk": "1980-1989",
            "prio": "6"
          },
          "437": {
            "characteristic_id": "437",
            "name": "1970-1979",
            "name_uk": "1970-1979",
            "prio": "5"
          },
          "438": {
            "characteristic_id": "438",
            "name": "1960-1969",
            "name_uk": "1960-1969",
            "prio": "4"
          },
          "439": {
            "characteristic_id": "439",
            "name": "1944-1959",
            "name_uk": "1944-1959",
            "prio": "3"
          },
          "440": {
            "characteristic_id": "440",
            "name": "1917-1942",
            "name_uk": "1917-1942",
            "prio": "2"
          },
          "441": {
            "characteristic_id": "441",
            "name": "раньше 1917",
            "name_uk": "до 1917",
            "prio": "1"
          },
          "442": {
            "characteristic_id": "442",
            "name": "не указано",
            "name_uk": "не вказано",
            "prio": "36"
          },
          "1448": {
            "characteristic_id": "1448",
            "name": "2014",
            "name_uk": "2014",
            "prio": "21"
          },
          "1449": {
            "characteristic_id": "1449",
            "name": "Сдача в 2015",
            "name_uk": "Здача в 2015",
            "prio": "30"
          },
          "1450": {
            "characteristic_id": "1450",
            "name": "Сдача в 2016",
            "name_uk": "Здача в 2016",
            "prio": "31"
          },
          "1454": {
            "characteristic_id": "1454",
            "name": "2015, III кв.",
            "name_uk": "2015, III кв.",
            "prio": "24"
          },
          "1455": {
            "characteristic_id": "1455",
            "name": "2015, II кв.",
            "name_uk": "2015, II кв.",
            "prio": "23"
          },
          "1456": {
            "characteristic_id": "1456",
            "name": "2015, I кв.",
            "name_uk": "2015, I кв.",
            "prio": "22"
          },
          "1457": {
            "characteristic_id": "1457",
            "name": "2016, I кв.",
            "name_uk": "2016, I кв.",
            "prio": "26"
          },
          "1458": {
            "characteristic_id": "1458",
            "name": "2016, II кв.",
            "name_uk": "2016, II кв.",
            "prio": "27"
          },
          "1459": {
            "characteristic_id": "1459",
            "name": "2016, III кв.",
            "name_uk": "2016, III кв.",
            "prio": "28"
          },
          "1460": {
            "characteristic_id": "1460",
            "name": "2016, IV кв.",
            "name_uk": "2016, IV кв.",
            "prio": "29"
          },
          "1468": {
            "characteristic_id": "1468",
            "name": "Сдача в 2017",
            "name_uk": "Здача в 2017",
            "prio": "32"
          },
          "1469": {
            "characteristic_id": "1469",
            "name": "Сдача в 2018",
            "name_uk": "Здача в 2018",
            "prio": "33"
          },
          "1470": {
            "characteristic_id": "1470",
            "name": "Сдача в 2019",
            "name_uk": "Здача в 2019",
            "prio": "34"
          },
          "1471": {
            "characteristic_id": "1471",
            "name": "Сдача в 2020",
            "name_uk": "Здача в 2020",
            "prio": "35"
          }
        },
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      }
    ]
  },
  {
    "group_name": "цена",
    "group_prio": 45,
    "items": [
      {
        "characteristic_id": 234,
        "label": "цена",
        "label_uk": "ціна",
        "type_on_add": "text",
        "type_on_search": "text",
        "data_type": "int",
        "required": 1,
        "characteristic_category": "main",
        "prio": 96,
        "name": "цена",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "group_prio": 64,
        "field_name": "price",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 1011,
        "label": "цена договорная",
        "label_uk": "ціна договірна",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 95,
        "name": "цена договорная",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "group_prio": 64,
        "field_name": "is_negotiable",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 242,
        "label": "тип валюты",
        "label_uk": "тип валюти",
        "type_on_add": "select",
        "type_on_search": "select",
        "data_type": "int",
        "required": 1,
        "default_value": "$",
        "characteristic_category": "main",
        "prio": 85,
        "name": "тип валюты (USD)",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "group_prio": 64,
        "children": {
          "239": {
            "characteristic_id": "239",
            "name": "$",
            "name_uk": "$",
            "prio": "3"
          },
          "240": {
            "characteristic_id": "240",
            "name": "грн",
            "name_uk": "грн",
            "prio": "2"
          },
          "241": {
            "characteristic_id": "241",
            "name": "€",
            "name_uk": "€",
            "prio": "1"
          }
        },
        "field_name": "currency_type",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      },
      {
        "characteristic_id": 1464,
        "label": "стартовая цена",
        "label_uk": "стартова ціна",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 45,
        "name": "стартовая цена",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "field_name": "start_price",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic",
        "group_prio": 0
      },
      {
        "characteristic_id": 273,
        "label": "возможен торг",
        "label_uk": "можливий торг",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 42,
        "name": "возможен торг",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "field_name": "is_bargain",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic",
        "group_prio": 0
      },
      {
        "characteristic_id": 274,
        "label": "возможна рассрочка / кредит",
        "label_uk": "можлива розстрочка / кредит",
        "type_on_add": "checkbox",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "characteristic_category": "main",
        "prio": 40,
        "name": "возможна рассрочка / кредит",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic",
        "group_prio": 0
      },
      {
        "characteristic_id": 265,
        "label": "возможен обмен",
        "label_uk": "можливий обмін",
        "type_on_add": "select",
        "type_on_search": "select",
        "data_type": "int",
        "required": 0,
        "default_value": "нет",
        "characteristic_category": "main",
        "prio": 35,
        "name": "возможен обмен",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "children": {
          "257": {
            "characteristic_id": "257",
            "name": "нет",
            "name_uk": "ні",
            "prio": "8"
          },
          "258": {
            "characteristic_id": "258",
            "name": "на авто + моя доплата",
            "name_uk": "на авто + моя доплата",
            "prio": "7"
          },
          "259": {
            "characteristic_id": "259",
            "name": "на авто без доплаты",
            "name_uk": "на авто без доплати",
            "prio": "6"
          },
          "260": {
            "characteristic_id": "260",
            "name": "на авто + ваша доплата",
            "name_uk": "на авто + ваша доплата",
            "prio": "5"
          },
          "261": {
            "characteristic_id": "261",
            "name": "на недвижимость + моя доплата",
            "name_uk": "на нерухомість + моя доплата",
            "prio": "4"
          },
          "262": {
            "characteristic_id": "262",
            "name": "на недвижимость без доплаты",
            "name_uk": "на нерухомість без доплати",
            "prio": "3"
          },
          "263": {
            "characteristic_id": "263",
            "name": "на недвижимость + ваша доплата",
            "name_uk": "на нерухомість + ваша доплата",
            "prio": "2"
          },
          "264": {
            "characteristic_id": "264",
            "name": "рассмотрю любой вариант",
            "name_uk": "розгляну будь-який варіант",
            "prio": "1"
          }
        },
        "field_name": "is_exchange",
        "display_label_search": 0,
        "display_label_add": 0,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic",
        "group_prio": 0
      },
      {
        "characteristic_id": 1437,
        "label": "тип предложения",
        "label_uk": "тип пропозиції",
        "type_on_add": "select",
        "type_on_search": "checkbox",
        "data_type": "int",
        "required": 0,
        "default_value": "от посредника",
        "characteristic_category": "main",
        "prio": 30,
        "name": "тип предложения",
        "group_name": "цена",
        "group_name_uk": "ціна",
        "group_prio": 64,
        "children": {
          "1434": {
            "characteristic_id": "1434",
            "name": "от посредника",
            "name_uk": "від посередника",
            "prio": "5"
          },
          "1435": {
            "characteristic_id": "1435",
            "name": "от представителя хозяина (без комиссионных)",
            "name_uk": "від представника власника (без комісійних)",
            "prio": "4"
          },
          "1436": {
            "characteristic_id": "1436",
            "name": "от собственника",
            "name_uk": "від власника",
            "prio": "2"
          },
          "1473": {
            "characteristic_id": "1473",
            "name": "от представителя застройщика",
            "name_uk": "від представника забудовника",
            "prio": "3"
          },
          "1506": {
            "characteristic_id": "1506",
            "name": "от застройщика",
            "name_uk": "від забудовника",
            "prio": "1"
          }
        },
        "display_label_search": 1,
        "display_label_add": 1,
        "group_orientation_search": "horisontal",
        "group_orientation_add": "horisontal",
        "empty_value": 0,
        "type": "characteristic"
      }
    ]
  }
]
```


## Информация по id объявления

Чтобы обратиться к  RIA API info, Вам необходимо выполнить GET запрос такого вида:

https://developers.ria.com/dom/info/**id_объявления**?api_key=YOUR_API_KEY

или  `curl -i -X GET "https://developers.ria.com/dom/info/id_объявления?api_key=YOUR_API_KEY"`

Полное описание сервиса "Информация по id объявления" описанный с помощью стандарта DeFacto swagger 2.0 [здесь](http://swagger.ria.com/ui/?api=dom/options)

Допусти Вам нужна информация по _13825265_ id.

Данный запрос будет выглядеть так:

https://developers.ria.com/dom/info/13825265?api_key=YOUR_API_KEY

или  `curl -i -X GET "https://developers.ria.com/dom/info/13825265?api_key=YOUR_API_KEY`

В случае успешного выполнения запроса  результат будет со статусом **200 OK**.

Пример успешного ответа:

```json
{
  "street_name": "Онуфрия Трутенко улица",
  "metro_station_id": "15",
  "rooms_count": 2,
  "advert_title": 1,
  "type": "realty",
  "is_commercial": 0,
  "state_name": "Киевская",
  "street_id": 5581,
  "state_id": 10,
  "beautiful_url": "realty-perevireno-prodaja-kvartira-kiev-goloseevskiy-onufriya-trutenko-ulitsa-13825265.html",
  "levels": 64,
  "exchange_required_type": 13,
  "district_type_name": "Район",
  "description": "Светлая квартира, расположена на 23 этаже / 23 эт. дома в ЖК &quot; 4 Сезона&quot;, потолок Н-3,5 м., панорамные окна с видом на город. Состояние от застройщика, у Вас есть возможность воплотить дизайнерские фантазии в доме. Дом имеет внешнее утепление, парковку, подземный паркинг, во дворе оборудованная детская площадка. Шикарный район, в шаговой дистанции м. &quot; Васильковская&quot; ( 5 мин.пешком), м. &quot;Ипподром&quot; (10 мин.пешком), м. &quot;Выстовочный Центр&quot;(18 мин. пешком)  Голосеевский парк,озёра  и пруды, детский сад, школа, магазины, салоны, кафе и рестораны, фитнес центр. ",
  "advert_publish_type": 1,
  "currency_type": "$",
  "district_type_id": 1,
  "longitude": "30.480281005166944",
  "inspected_at": "2017-10-02 14:51:02",
  "levels_expired": "2018-01-01 12:16:32",
  "is_exchange": "рассмотрю любой вариант",
  "district_id": "15184",
  "metro_station_name": "Васильковская",
  "wall_type": "кирпич",
  "publishing_date": "2017-10-02 14:51:07",
  "description_uk": "Світла квартира, розташована на 23 поверсі / 23 пов. будинки в ЖК &quot;4 Сезони&quot;, стеля Н-3,5 м., панорамні вікна з видом на місто. Стан від забудовника, у Вас є можливість втілити дизайнерські фантазії в будинку. Будинок має зовнішнє утеплення, місце для паркування, підземний паркінг, у дворі обладнаний дитячий майданчик. Шикарний район, в крокової дистанції м. &quot;Васильківська&quot; ( 5 хв. пішки), м. &quot;Іподром&quot; (10 хв. пішки), м. &quot;Вистовковий Центр&quot;(18 хв. пішки), Голосіївський парк, озера і ставки, дитячий садок, школа, магазини, салони, кафе і ресторани, фітнес-центр.  ",
  "youtube_link": "",
  "price_type": "за объект",
  "inspected": 1,
  "is_bargain": 273,
  "price": 60000,
  "floor": 23,
  "latitude": "50.39161687881484",
  "price_total": 60000,
  "main_photo": "dom/photo/8070/807045/80704539/80704539.jpg",
  "price_item": 645,
  "realty_type_name": "Квартира",
  "building_number_str": "3 Г",
  "city_name": "Киев",
  "metro_station_brunch": 2,
  "realty_type_parent_id": 1,
  "living_square_meters": 50,
  "realty_type_id": 2,
  "user_ip": 0,
  "city_id": 10,
  "characteristics_values": {
    "118": 108,
    "209": 2,
    "214": 93,
    "216": 50,
    "218": 20,
    "227": 23,
    "228": 23,
    "234": 60000,
    "242": 239,
    "247": 252,
    "265": 264,
    "273": 273,
    "443": 1449,
    "475": 473,
    "480": 476,
    "516": 512,
    "791": 791,
    "806": 802,
    "808": 808,
    "892": 890,
    "1016": 1016,
    "1020": 1023,
    "1032": 1028,
    "1157": 1149,
    "1403": 1400,
    "1437": 1436,
    "1504": 1504,
    "1571": 1571,
    "1575": 1575,
    "1581": 1581
  },
  "_id": "realty-13825265",
  "floors_count": 23,
  "created_at": "2017-09-20 21:12:42",
  "user_id": 7160632,
  "kitchen_square_meters": 20,
  "user_package_id": 0,
  "total_square_meters": 93,
  "realty_id": 13825265,
  "realty_sale_type": 2,
  "photos": {
    "80704539": {
      "id": 80704539,
      "file": "dom/photo/8070/807045/80704539/80704539.jpg",
      "o": "h"
    },
    "80704540": {
      "id": 80704540,
      "file": "dom/photo/8070/807045/80704540/80704540.jpg",
      "o": "h"
    },
    "80704541": {
      "id": 80704541,
      "file": "dom/photo/8070/807045/80704541/80704541.jpg",
      "o": "h"
    },
    "80704542": {
      "id": 80704542,
      "file": "dom/photo/8070/807045/80704542/80704542.jpg",
      "o": "h"
    },
    "80704543": {
      "id": 80704543,
      "file": "dom/photo/8070/807045/80704543/80704543.jpg",
      "o": "v"
    },
    "80704545": {
      "id": 80704545,
      "file": "dom/photo/8070/807045/80704545/80704545.jpg",
      "o": "v"
    },
    "80704546": {
      "id": 80704546,
      "file": "dom/photo/8070/807045/80704546/80704546.jpg",
      "o": "v"
    },
    "80704547": {
      "id": 80704547,
      "file": "dom/photo/8070/807045/80704547/80704547.jpg",
      "o": "v"
    },
    "80704548": {
      "id": 80704548,
      "file": "dom/photo/8070/807045/80704548/80704548.jpg",
      "o": "v"
    },
    "80704550": {
      "id": 80704550,
      "file": "dom/photo/8070/807045/80704550/80704550.jpg",
      "o": "h"
    },
    "80704552": {
      "id": 80704552,
      "file": "dom/photo/8070/807045/80704552/80704552.jpg",
      "o": "h"
    }
  },
  "date_end": "2018-03-02 14:51:07",
  "district_name": "Голосеевский",
  "advert_type_id": 1,
  "advert_type_name": "продажа",
  "is_show_building_no": 1,
  "realty_type_parent_name": "Квартиры",
  "user": {
    "name": "Владимир",
    "image": "",
    "good_partner_top": ""
  },
  "priceArr": {
    "1": "60 000",
    "2": "50 588",
    "3": "1 680 672"
  },
  "with_panoramas": 1
}
```

## Поиск объявлений

Чтобы обратиться к  DOM.RIA API search, Вам необходимо выполнить GET запрос такого вида:

https://developers.ria.com/dom/search?api_key=YOUR_API_KEY&PARAMETERS

или `curl -X GET "https://developers.ria.com/dom/search?api_key=YOUR_API_KEY&PARAMETERS"  -H "accept: application/json"`

Он состоит из:

 * **SEARCH** — название метода API, к которому Вы хотите обратиться.

 * **API_KEY** — ключ доступа. Для получения ключа доступа нужно зарегестрироватся на портале developers.ria.com 

 * **PARAMETERS** — входные параметры, последовательность пар name=value, разделенных амперсандом. Список параметров указан выше.

В ответ на такой запрос Вы получите ответ в формате JSON:

```json
{
  "items": [                //id объявлений
    
  ],
  "count":                // количество
}
```

Полное описание сервиса "Поиск объявлений" описанный с помощью стандарта DeFacto swagger 2.0
* [Квартир](http://swagger.ria.com/ui/?api=dom/apartments)
* [Домов](http://swagger.ria.com/ui/?api=dom/house#/)
* [Коммерческой недвижимости](http://swagger.ria.com/ui/?api=dom/commercial)
* [Офисов](http://swagger.ria.com/ui/?api=dom/offices)
* [Земельных участков](http://swagger.ria.com/ui/?api=dom/land)
* [Гаражей](http://swagger.ria.com/ui/?api=dom/garages)


**Пример**

Допустим Вы ищете:
* Объект - Квартиры
* Тип недвижимости - квартира
* Операция - продажа
* Область - Киевская
* Город - Киев
* Район
   * Оболонский
   * Печерский
   * Подольский
* Количество комнат от 1 до 3
* Общая площадь от 60 до 90
* Жилая площадь от 30 до 50
* Кухня от 4 до 9
* Кухня от 3 до 7
* Год постройки - не указан
* Цена от 20000 до 90000
* Цена за объект
* Тип валюты долары США
* Возможен торг
* Тип предложения - от посредника


В итоге мы получаем запрос такого [вида]:

[https://developers.ria.com/auto/search?api_key=YOUR_API_KEY&category=1&realty_type=2&operation_type=1....](https://developers.ria.com/dom/search?category=1&realty_type=2&operation_type=1&state_id=10&city_id=10&district_id=15187&district_id=15189&district_id=15188&characteristic[209][from]=1&characteristic[209][to]=3&characteristic[214][from]=60&characteristic[214][to]=90&characteristic[216][from]=30&characteristic[216][to]=50&characteristic[218][from]=4&characteristic[218][to]=9&characteristic[227][from]=3&characteristic[227][to]=7&characteristic[443]=442&characteristic[234][from]=20000&characteristic[234][to]=90000&characteristic[242]=239&characteristic[273]=273&characteristic[1437]=1434&api_key=YOUR_API_KEY)

или `curl -X GET "https://developers.ria.com/dom/search?category=1&realty_type=2&operation_type=1&state_id=10&city_id=10&district_id=15187&district_id=15189&district_id=15188&characteristic[209][from]=1&characteristic[209][to]=3&characteristic[214][from]=60&characteristic[214][to]=90&characteristic[216][from]=30&characteristic[216][to]=50&characteristic[218][from]=4&characteristic[218][to]=9&characteristic[227][from]=3&characteristic[227][to]=7&characteristic[443]=442&characteristic[234][from]=20000&characteristic[234][to]=90000&characteristic[242]=239&characteristic[273]=273&characteristic[1437]=1434&api_key=YOUR_API_KEY" -H "accept: application/json"`

В случае успешного выполнения запроса по указанным параметрам результат будет со статусом **200 OK**.

Пример успешного ответа:

```json
{
  "items": [
    13336044,
    14076392,
    13814523,
    14064249,
    13078930,
    13927706,
    13962022
  ],
  "count": 7
}
```


## Методы для работы с областями, городами, районами
### Области
Получить список областей можно отправив GET запрос по адресу [https://developers.ria.com/dom/states?api_key=YOUR_API_KEY](https://developers.ria.com/dom/states?api_key=YOUR_API_KEY).
Для получение информации на украинском языке нужно добавить параметр *lang_id=4*

Полное описание сервиса "Методы для работы с областями, городами, районами" описанный с помощью стандарта DeFacto swagger 2.0 [здесь](http://swagger.ria.com/ui/?api=dom/states_cities_and_districts)

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
  
###Города
  
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

###Районы

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