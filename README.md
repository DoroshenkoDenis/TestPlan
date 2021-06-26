# План тестирования возможности записи на обучение профессии "Тестировщик ПО"

## 1. Введение
___

## 2. Виды тестирования
* Функциональное тестирование формы записи
___

## 3. Перечень автоматизируемых сценариев   
### **Предусловие 1 "Неавторизованный пользователь" / "RegisrationCard":**
* Перейти к форме записи RegisrationCard
 ![RegisrationCardNoRegistratedUser](https://user-images.githubusercontent.com/47859608/123509358-0b640c80-d686-11eb-8562-9326330e70f0.png)
**Способы перехода**
1. "programmBlock"
   * Перейти на сайт [Нетология](https://netology.ru/);
   * В Header нажать кнопку "Каталог курсов"
   * В Navigator нажать "Программирование"
   * Нажать в programmBlock модуль "Тестировщик ПО" 
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Нажать "Записаться" в начале страницы или в тулбаре при скроле вверх 
2. "Для начинающих"
   * В Header нажать кнопку "Каталог курсов"
   * В Navigator навести на "Программирование"
   * Справа в колонке "Для начинающих" нажать "Тестировщик ПО" 
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Нажать "Записаться" в начале страницы или в тулбаре при скроле вверх 
3. "Banner"
   * В Banner нажать кнопку "Подробнее"
   * В открывшемся фрейме нажать "Выбрать курс"
   * Установить курсор в поле "Поиск"
   * В полученном списке выбрать "Тестировщик ПО"
   * Нажать в programmBlock модуль "Тестировщик ПО"
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Нажать "Записаться" в начале страницы или в тулбаре при скроле вверх
4. "Banner - Поиск"
   * В Header нажать кнопку "Каталог курсов"
   * В Banner нажать кнопку "Подробнее"
   * В открывшемся фрейме нажать "Выбрать курс"
   * Установить курсор в поле "Поиск"
   * Ввести в поле "Тестировщик ПО" и нажать поиск
   * Нажать в programmBlock модуль "Тестировщик ПО" внизу в результатах поиска 
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Нажать "Записаться" в начале страницы или в тулбаре при скроле вверх
5. "НЕО для начинающих"
   * Нажать ссылку "НЕО для начинающих"
   * Установить галочку в CheckBox "Программирование"
   * В полученном programmBlock выбрать модуль "Тестировщик ПО"
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Нажать "Записаться" в начале страницы или в тулбаре при скроле вверх
6. "Актуальные темы"
   * Скролить вниз
   * В списке "Актуальные темы" выбрать "Программирование"
   * В полученном programmBlock выбрать модуль "Тестировщик ПО"
   * Получить страницу ["Тестировщик"](https://netology.ru/programs/qa)
   * Нажать "Записаться" в начале страницы или в тулбаре при скроле вверх

### **Предусловие 2 "Неавторизованный пользователь" / "Modalbox":**
* Перейти к форме записи ModalBox
![ModalBoxNoRegistratedUser](https://user-images.githubusercontent.com/47859608/123509367-1c148280-d686-11eb-9aac-aed1e35795df.png)
**Способы перехода**
  * Переход к странице специальности аналогично "Предусловие 1"
  * В контейнере "Гарантия возврата денег" нажать "Записаться"

### **Предусловие 3 "Авторизованный пользователь" / "RegisrationCard":**
* Перейти к форме записи RegisrationCard
![RegisrationCardRegistratedUser](https://user-images.githubusercontent.com/47859608/123509441-a0ff9c00-d686-11eb-9360-d8dc01bc8a03.png)
**Способы перехода**
  * Перейти на сайт [Нетология](https://netology.ru/);    
  * В Header нажать кнопку "Войти"
  * Авторизоваться через сторонний ресурс / Авторизоваться через поля "e-mail" & "password"
  * Остальные шаги аналогично "Предусловие 1"
  
### **Предусловие 4 "Авторизованный пользователь" / "Modalbox":**
* Перейти к форме записи Modalbox
![ModalBoxRegistratedUser](https://user-images.githubusercontent.com/47859608/123509448-aa890400-d686-11eb-83ba-37b2a2879c70.png)
**Способы перехода**
  * Перейти на сайт [Нетология](https://netology.ru/);    
  * В Header нажать кнопку "Войти"
  * Авторизоваться через сторонний ресурс / Авторизоваться через поля "e-mail" & "password"
  * Остальные шаги аналогично "Предусловие 2"
___

      *  Заполнить поле Имя 
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"
   * проверить ожидаемый результат - сообщение об успешной записи

  * Заполнить форму Modalbox
      *  Заполнить поле Имя
      *  Заполнить поле Телефон
      *  Заполнить поле e-mail
      *  Нажать "Записаться"
___
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
___
* **Итого:** 16 часов
