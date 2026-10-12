# СпортТовары — система управления магазином

---

## Описание

Учебный проект — консольное приложение для управления магазином спортивных товаров. Позволяет вести каталог, искать товары, работать с корзиной, оформлять заказы и просматривать аналитику по продажам.

---

## Требования

* Python 3.10+
* Git
* **SQLite не используется — данные хранятся в JSON (`data/products.json`, `data/orders.json`)**

---

## Установка

```bash
git clone git@github.com:Belomaster/SportShop.git
cd SportShop


## Запуск
python3.12 main.py

##Тестирование
python3.12 -m unittest discover -s tests -v
Ожидаемый результат: Ran 23 tests ... OK.

## Сборка
python3.12 build.py

## Структура проекта

```text
SportShop/
├── src/
│   ├── __init__.py
│   ├── catalog.py          # работа с каталогом товаров
│   ├── cart.py             # корзина покупателя
│   ├── orders.py           # заказы
│   ├── analytics.py        # аналитика по заказам
│   └── storage.py          # сохранение/загрузка JSON
├── tests/
│   ├── __init__.py
│   ├── test_shop.py        # модульные тесты
│   └── test_integration.py # интеграционные тесты
├── docs/                   # документация проекта
├── data/
│   └── products.json       # данные о товарах
├── main.py                 # точка входа
├── build.py                # скрипт сборки
└── README.md

## Использование

После запуска `main.py` откроется консольное меню:

```text
=== SportShop ===
1. Показать все товары
2. Товары с низким остатком
3. Поиск
4. Аналитика по категориям
5. Средняя цена
6. Добавить в корзину
7. Показать корзину / сумму
8. Оформить заказ
9. Аналитика по заказам
0. Выход

Выбор: 3
Запрос: nike
{'id': 1, 'name': 'Мяч Nike', 'brand': 'Nike', 'category': 'Игры', 'price': 1500, 'quantity': 5}

## Документация

* [API Reference](https://github.com/Belomaster/SportShop/blob/main/docs/17_API_Reference.md)
* [User Guide](https://github.com/Belomaster/SportShop/blob/main/docs/18_User_Guide.md)
* [Developer Guide](https://github.com/Belomaster/SportShop/blob/main/docs/19_Developer_Guide.md)
* [Final Test Report](https://github.com/Belomaster/SportShop/blob/main/docs/20_Final_Test_Report.md)
* [Presentation](https://github.com/Belomaster/SportShop/blob/main/docs/21_Presentation.md)

---

## Авторы

* yakimenkodaniil — разработка, тестирование, документация (учебный проект, 2026)

---

## Лицензия

Учебный проект. Свободное использование в образовательных целях.
