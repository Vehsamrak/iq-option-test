# ТЗ

Есть два компонента А и Б. Необходимо обеспечить общение обоих этих компонентов через шину данных (шина данных на выбор исполнителя). Компонент А генерирует сообщения разных версий, а компонент Б слушает только те версии сообщений, на которые он подписался. Нужно предусмотреть возможность масштабирования компонента Б в случае роста количества отправляемых сообщений компонентом А. Компонент Б также должен сохранять полученные данные в базу.

Пример сообщения (json):

```
{
    "name": "EUR/USD",
    "value": 1.3023421,
    "time": 1465312662
}
```

name - название котировки (выбрать несколько значений)
value - значение котировки (случайное число в интервале от 1 до 2)
time - время в формате unix timestamp