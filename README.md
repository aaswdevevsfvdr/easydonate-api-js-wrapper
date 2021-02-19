# EasyDoante API Wrapper
API Wrapper для взаимодействия с easydonate.ru
## Подключение

``` js
const {
    EasyDonate
} = require('easydonate-api')
const api = new EasyDonate({"token": process.env.TOKEN })
```

## Методы API
***getShopInfo*** - получить информацию о магазине

**Пример**
``` js
async function getShopInfo() {
let shop = api.getShopInfo() 
console.log(shop)
}
getShopInfo().catch(console.error)
```

***getShopProducts*** - получить все товары магазина

**Пример**
``` js
async function getShopProducts() {
let products = mc.getShopProducts() 
console.log(products)
}
getShopProducts().catch(console.error)
```

***getProductInfo*** - получить информацию о продукте
| Параметр | Тип | Обязателен | Описание |
|--|--|--|--|
| id | number | Да | ID продукта |

**Пример**
``` js
async function getProductInfo() {
let product = mc.getProductInfo(1234) 
console.log(product)
}
getProductInfo().catch(console.error)
```

***getShopServers*** - получить все сервера магазина

**Пример**
``` js
async function getShopServers() {
let servers = mc.getShopServers() 
console.log(servers)
}
getShopServers().catch(console.error)
```

***getServerInfo*** - получить информацию о сервере
| Параметр | Тип | Обязателен | Описание |
|--|--|--|--|
| id | number | Да | ID сервер |

**Пример**
``` js
async function getServerInfo() {
let server = mc.getServerInfo(1234) 
console.log(server)
}
getServerInfo().catch(console.error)
```


