# План проверки мобильного приложения "Мобильный хоспис" или "Вхосписе".

---

## Описание приложения:

#### Приложение даёт функционал по работе с претензиями хосписа и включает в себя:

- информацию о претензиях и функционал для работы с ними;
- новостную сводку хосписа;
- тематические цитаты.

---

## Границы приложения и реализованный функционал:

1. Страница авторизации

- Поле для ввода Login
- Поле для ввода Password
- Кнопка Sign in

2. Главный экран

2.1. Кнопки верхней панели
- Меню, состоящее из разделов (Main, News, About)
- Вкладка Love is all с тематическими цитатами
- Кнопка выхода (Logout)

2.2. Основной экран (по умолчанию открыт Main)
- Раздел News, с разворотом и переходом на ALL NEWS

---
## Тест-план для проверки приложения:

#### Проверка экрана авторизации
    1. Проверка валидных/невалидных значений.
    2. Проверка регистрации с верными/ощибочными данными.

#### Проверка экрана "Main"
      - Отображение блока новостей
      - Отображение блока претензий
      - Сворачивание/разворачивание блока новостей
      - Сворачивание/разворачивание блока претензий
      - Сворачивание/разворачивание отдельной новости
      - Сворачивание/разворачивание отдельной претензии
      - Создание претензии

#### Проверка экрана "News", через переход в "ALL NEWS"
      - Сворачивание/разворачивание отдельной новости
      - Порядок отображения новостей
      - Фильтрация новостей
      - Переход к редактированию новостей, через control panel:
        - Сворачивание/разворачивание отдельной новости
        - Порядок отображения новостей
        - Фильтрация новостей
        - Создание новости
        - Редактирование новости
        - Удаление новости

#### Проверка экрана "About"
      - Отображение версии приложения
      - Отображение правил использования
      - Отображение политики конфиденциальности
      - Открытие ссылки "Terms of use"
      - Открытие ссылки "Privacy Policy"

#### Проверка экрана "Love is all" с цитатами
      - Сворачивание/разворачивание отдельной цитаты

#### Проверка переходов между экранами

#### Проверка выхода из приложения

---

## Виды тестирования:

- Ручное
- Автоматизированное

- Функциональное:
    - все проверки по тест-плану
- Нефункциональное:
    - установочное тестирование
    - Usability тестирование
  
---

# Инструменты тестирования и автоматизации:

### Ручное тестирование:
- **Android Studio**: Для эмуляции мобильного устройства и запуска приложения на эмуляторе. Выбран из-за удобства эмуляции различных устройств с разными версиями Android.
- **Google Sheets**: Для создания чек-листа и тест-кейсов. Удобный инструмент для организации и отслеживания тестовой документации.
- **Браузер для проверки ссылок**: Для проверки работоспособности ссылок на странице "About". Браузер выбирается на усмотрение тестировщика, но рекомендуется использовать популярные браузеры, такие как Chrome или Firefox.

### Автоматизированное тестирование:
- **Appium**: Для автоматизации тестирования мобильных приложений. Appium выбран из-за его кросс-платформенности и возможности работы с различными языками программирования.
- **Selenium WebDriver**: Для автоматизации тестирования веб-интерфейса приложения. Selenium WebDriver широко используется в индустрии и имеет обширное сообщество поддержки.

### Автоматизируемые сценарии:
- Автоматизация проверки экрана авторизации: ввод валидных и невалидных данных, проверка регистрации.
- Автоматизация проверки экрана "Main": отображение блока новостей и претензий, сворачивание/разворачивание блоков, создание претензии.
- Автоматизация проверки экрана "News" и "ALL NEWS": сворачивание/разворачивание отдельной новости, фильтрация новостей, создание, редактирование и удаление новости.
- Автоматизация проверки экрана "About": отображение версии приложения, правил использования, политики конфиденциальности, а также проверка работоспособности ссылок.
- Автоматизация проверки экрана "Love is all" с цитатами: сворачивание/разворачивание отдельной цитаты.
- Проверка переходов между экранами.
- Проверка выхода из приложения.

## Интервальная оценка:

### Ручное тестирование:
Предполагаем, что ручное тестирование каждого из пунктов плана займет примерно 3 часа. Учитывая общий объем плана (7 пунктов), общая оценка составляет примерно 21 час.

### Автоматизированное тестирование:
Сложность автоматизации зависит от доступности элементов управления и структуры приложения. Предположим, что автоматизация каждого из сценариев займет примерно 5 часов. Таким образом, общая оценка для автоматизации составит примерно 35 часов.

### Общая оценка на тестирование и автоматизацию:
56 часов. Учитывая потенциальные риски и необходимость дополнительного времени на отладку и исправление найденных дефектов, рекомендуется увеличить общую оценку на 20%, что составит примерно 67 часов.

___
## Окружение:

Ноутбук: HP Laptop 15s, процессор AMD Ryzen 3 5300U, оперативная память 16гб / Операционная система: Windows 11 Pro, 64-разрядная.
Мобильное устройство: 5.5" Эмулятор смартфона Pixel XL API 29/ Версия Android: 10 / Разрешение: 1440x2560.

---

## Тестовая документация:

**Чек-лист:** https://docs.google.com/spreadsheets/d/15YJiOt0RNHwI1rGuOKl2lF_f2KUyFNNZ/edit#gid=1474013527

**Тест-кейсы:** https://docs.google.com/spreadsheets/d/1vHjyPISd3-K1KHmxQdC4k0CNVebzVVw9/edit#gid=716714085