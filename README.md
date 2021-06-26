# План тестирования возможности записи на обучение профессии "Тестировщик ПО"

## Введение

## Вид тестирования
* Функциональное тестирование формы записи
* EmptyFields - ожидаемый результат - сообщение "Обязательное поле"
* WrongChar - ожидаемый результат - сообщение "Должно состоять из букв" / "Номер в формате +9 (999) 999-99-99"

## Перечень автоматизируемых сценариев 
### Сценарий - 1: "Неавторизованный пользователь"  
**Предусловие:**
* Перейти на сайт [Нетология](https://netology.ru/);
* Перейти к форме регистрации ![Image of RegisrationCard](https://user-images.githubusercontent.com/47859608/123507805-96400980-d67c-11eb-975f-b3ddc3010052.png)
* 
* Способы перехода



* Сценарий - 1.1 "programmBlock"
   * В Header нажать кнопку "Каталог курсов"
   * В Navigator нажать "Программирование"
   * Нажать в programmBlock модуль "Тестировщик ПО" 
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Заполнить форму RegisrationCard (перейти к форме можно нажав кнопку "Записаться" в начале страницы и в тулбаре при скроле вверх)
      *  Заполнить поле Имя 
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"
   * проверить ожидаемый результат - сообщение об успешной записи

* Сценарий - 1.2 "Для начинающих"
   * В Header нажать кнопку "Каталог курсов"
   * В Navigator навести на "Программирование"
   * Справа в колонке "Для начинающих" нажать "Тестировщик ПО" 
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Заполнить форму RegisrationCard
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"

* Сценарий - 1.3 "Banner"
   * В Banner нажать кнопку "Подробнее"
   * В открывшемся фрейме нажать "Выбрать курс"
   * Установить курсор в поле "Поиск"
   * В полученном списке выбрать "Тестировщик ПО"
   * Нажать в programmBlock модуль "Тестировщик ПО"
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Заполнить форму RegisrationCard
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться" 

* Сценарий - 1.4 "Banner - Поиск"
   * В Header нажать кнопку "Каталог курсов"
   * В Banner нажать кнопку "Подробнее"
   * В открывшемся фрейме нажать "Выбрать курс"
   * Установить курсор в поле "Поиск"
   * Ввести в поле "Тестировщик ПО" и нажать поиск
   * Нажать в programmBlock модуль "Тестировщик ПО" внизу в результатах поиска 
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Заполнить форму RegisrationCard
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"

* Сценарий - 1.5 "НЕО для начинающих"
   * Нажать ссылку "НЕО для начинающих"
   * Установить галочку в CheckBox "Программирование"
   * В полученном programmBlock выбрать модуль "Тестировщик ПО"
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Заполнить форму RegisrationCard
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"

* Сценарий - 1.6 "Актуальные темы"
   * Скролить вниз
   * В списке "Актуальные темы" выбрать "Программирование"
   * В полученном programmBlock выбрать модуль "Тестировщик ПО"
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Заполнить форму RegisrationCard
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"
      
* Сценарий - 1.7 "Гарантия возврата денег - Modalbox"
  * Выполнить любой сценарий до получения страницы ["Тестировщик"](https://netology.ru/programs/qa)
  * В контейнере "Гарантия возврата денег" нажать "Записаться"
  * Заполнить форму Modalbox
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"

### Сценарий 2: "Авторизованный пользователь"
**Предусловие:** Перейти на сайт [Нетология](https://netology.ru/);    
* В Header нажать кнопку "Войти"
* Авторизоваться через сторонний ресурс / Авторизоваться через поля "e-mail" & "password"
* Остальные шаги аналогично "Сценарий - 1" **без заполнения поля e-mail**

## Перечень используемых инструментов:
* Java 11 - версия в которой разрабатывается ПО;
* IntelliJ IDEA - удобная среда разработки для JAVA;
* Gradle - популярная система автоматической сборки;
* JUnit 5 - вложенные и параметризованные тесты;
* Selenide - управление браузером и создание автоматических скриншотов;
* Faker - генерация пользовательских данных;
* Docker - система для быстрого развёртывания и перезапуска базы данных.
* Git - система контроля версий.
* GitHub - удалённое хранилище проекта.
* Reporting.Allure - автоматическое создание отчётов.
* GitHub.Actions - система CI CD.

## Перечень необходимых разрешений/данных/доступов
* Разрешение ответственного лица организации ООО «Нетология» на проведение тестирования
* Доступ к API (токены / документация)
* Доступ к БД
* ac/dc power up

## Перечень и описание возможных рисков при автоматизации
* Высокая стоимость используемых инструментов
* Большие сроки написания тестов, возможна потеря актуальности некоторых тестов (банер) 
* Необходимость поддержки тестов

## Перечень необходимых специалистов для автоматизации
Automation QA Engineer - 1 

## Интервальная оценка с учётом рисков (в часах)
* Уточнение требований, cогласования и получение разрешений - 2 часа;
* Развёртывание окружения - 2 часа;
* Написание авто-тестов - 8 часов;
* Баг-репорты - 1 час;
* Подготовка отчета о тестировании - 2 часа;
* Подготовка отчета о проделанной работе - 1 час.
-----------------------------------------------
* **Итого:** 16 часов
