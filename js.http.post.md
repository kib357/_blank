# http.post

Метод `http.post()` выполняет POST запрос на указанный URL.

## Синтаксис

```
http.post(uri[, params])
```

## Параметры

### uri
Адрес запроса (строка). Слэши следует экранировать.

### params
Данные для выполнения запроса, которые будут отправлены как форма (объект, опционально). 

```
{
    param: "value"
}
```

## Возвращаемые значения

Объект вида:

```
{
    header: {
        header1: ['value'],
        header2: ['value2', 'value3']
    },
    statusCode: 200,
    body: 'RESULT'
}
```

## Пример  

```
var params = {
    param: 'yaya.ru',
    param2: 'neya.ru'
};
http.post('http:\/\/yandex.ru', params);
```
