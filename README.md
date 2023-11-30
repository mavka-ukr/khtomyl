# Хтомиль

Щось для створення вебсайтів Мавкою.

## Підключення

```мавка
взяти "хтомиль/0.3.0"
```

## Структура

```мавка
структура Хтомиль
  сторінки словник = ()
кінець
```

## Використання

### Сервер

```мавка
взяти "хтомиль/0.3.0"
взяти "хтомиль/0.3.0/сервер" як хтомиль_сервер

індекс = (
  відмалювати=дія()
    "Привіт від Лесі!"
  кінець
)

х = хтомиль.Хтомиль((
  ""=індекс
))

хтомиль_сервер.запустити(
  х,
  (порт=8080),
  (): друк("Сервер запущено на http://localhost:8080!")
)
```

### Генератор

```мавка
взяти "хтомиль/0.3.0"
взяти "хтомиль/0.3.0/генератор" як хтомиль_генератор

індекс = (
  відмалювати=дія()
    "Привіт від Лесі!"
  кінець
)

х = хтомиль.Хтомиль((
  ""=індекс
))

чекати хтомиль_генератор.згенерувати(х)
```