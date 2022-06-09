# Проект по курсу в РТУ МИРЭА
## Описани
Shaurmados - сервис для заказа шаурмы.

## Оглавление
1. [Структура проекта](#ref1)
1. [Как это должно работать?](#ref2)
1. [Архитектура проекта](#ref3)
## Содержание

### <a name="ref1"></a> 1. Структура проекта

Приложение состоит из следующих частей:
1. База данных - PostgreSQL
2. Backend - Spring Framework
3. UI - веб сайт

### <a name="ref2"></a> 2. Как это должно работать?


**Пример использования**

Пользователь желает создать заказ.

Тогда пользователь заходит на сайт, нажимает кнопку "сформировать заказ", выбирает нужные пиццы, выбирает, нужна ли доставка и осуществляет заказ. 

UI может выглядеть следующим образом:

![image](https://sun9-72.userapi.com/s/v1/if2/Ol3lCy1O2edWZ2vMJfAg-boEsfs4UmZ9mWXDVh8NtxCSUzKGm8yt6kRnd9Sym1TJmYt8S4rQmPprZoqrMvV7qvR7.jpg?size=2560x1303&quality=96&type=album)

### <a name="ref3"></a> 3. Архитектура проекта

Структура:
- База данных / Хранилище готовых данных
  - PostgreSQL
- Сервер
  - Абстракция для сущности данных
  - Сервисы
  - Модели
  - Контроллеры
  - Репозитории для взаимодействия с БД
  - Конвертер данных
- Клиент
  - Поля для ввода
  - Вывод информации
  - Нужные страницы
