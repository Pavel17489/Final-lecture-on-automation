## План тестирования возможности записи на обучение профессии ["Инженер по тестированию"](https://netology.ru/programs/qa-middle).

### 1.Перечень автоматизируемых сценариев:

#### Предусловия:

Переход к форме записи на курс "Инженер по тестированию":

- Открыть страницу сайта Нетология (https://netology.ru/)

- К форме записи на курс существует несколько способов перехода:

1. В левом верхнем углу нажать на кнопку `"Каталог курсов"`, нажать на категорию `"Программирование"`, нажать на курс `"Инженер по тестированию"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

2. На главной странице веб-сайта Нетология нажать на категорию `"Программирование"`, нажать на курс `"Инженер по тестированию"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

3. На главной странице веб-сайта Нетология нажать на категорию `"Программирование"`, в поле поиска `"Какой курс вам нужен?"` ввести "Инженер по тестированию", нажать на курс `"Инженер по тестированию: расширенный курс"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

4. В левом верхнем углу нажать на кнопку `"Каталог курсов"`, в поле поиска `"Какой курс вам нужен?"` ввести "Инженер по тестированию", нажать на курс `"Инженер по тестированию: расширенный курс"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

5. На главной странице веб-сайта Нетология нажать на кнопку `"Освоить профессию"`, нажать на категорию `"Программирование"`, нажать на курс `"Инженер по тестированию"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

6. На главной странице веб-сайта Нетология нажать на кнопку `"Освоить профессию"`, в поле поиска `"Какой курс вам нужен?"` ввести "Инженер по тестированию", нажать на курс `"Инженер по тестированию: расширенный курс"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

7. На главной странице веб-сайта Нетология нажать на кнопку `"Освоить профессию"`, нажать на категорию `"Программирование"`, в поле поиска `"Какой курс вам нужен?"` ввести "Инженер по тестированию", нажать на курс `"Инженер по тестированию: расширенный курс"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

8. В футере главной страницы веб-сайта Нетология нажать на кнопку `"Программирование"` в графе `"Обучение"`, нажать на курс `"Инженер по тестированию"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

9. В левом верхнем углу нажать на кнопку `"Каталог курсов"`, нажать на категорию `"Программирование"`, справа в меню страницы отметить чек-бокс `"Тестирование ПО"` в разделе `"Навыки"`, нажать на курс `"Инженер по тестированию"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

10. На главной странице веб-сайта Нетология нажать на кнопку `"Полный каталог"`, нажать на курс `"Инженер по тестированию"`, нажать на кнопку `"Записаться"`, происходит автоматический проскролл к форме записи на курс.

#### Тестовые сценарии:

##### Позитивные:

###### Пользователь не зарегистрирован или не авторизован на сайте

- В поле "Имя" ввести валидное значение имени: короткое имя, длинное имя, имя в нижнем регистре, имя в верхнем регистре, двойное имя через дефис, двойное имя через пробел, имя с буквой ё, имя на кириллице, имя на латинице.
- В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
- В поле "Электронная почта" ввести валидное значение электронной почты: Email в нижнем регистре, Email в верхнем регистре, Email с цифрами в имени аккаунта или в доменной части, Email с дефисом в имени аккаунта или доменной части, Email с точками в имени аккаунта, Email с несколькими точками в доменной части.

**Ожидаемый результат:** На электронный адрес приходит письмо с подтверждением заявки. Переход на страницу оплаты.

###### Пользователь зарегистрирован и авторизован на сайте

- В поле "Имя" ввести действительное значение имени: короткое имя, длинное имя, имя в нижнем регистре, имя в верхнем регистре, двойное имя через дефис, двойное имя через пробел, имя с буквой ё, имя на кириллице, имя на латинице.
- В поле с номером телефона введите действительное значение для номера телефона: номер в формате +9 (999) 999-99-99.

**Ожидаемый результат:** На зарегистрированный адрес электронной почты приходит письмо с подтверждением заявки. Переход на страницу оплаты.

##### Негативные:

1. Оставить поле/поля формы/форм пустыми.
**Ожидаемый результат:**  форма не отправляется, поле/поля подсвечиваются с ошибкой "Обязательное поле".
2. Заполнить поле "Имя" не валидными данными (спец.символы в имени, иероглифы вместо кириллицы или латиницы, пробелы вместо букв).
**Ожидаемый результат:** Появляется сообщение об ошибке под полем "Имя" красным цветом: "Должно состоять из букв"
3. Заполнить поле "Имя" не валидными данными (одна буква).
**Ожидаемый результат:** Появляется сообщение об ошибке под полем "Имя" красным цветом: "Должно быть не короче 2 символов"
4. Заполнить поле "Номер телефона" не валидными данными (номер телефона без знака + в начале, номер телефона более/менее 11 цифр).
**Ожидаемый результат:** Появляется сообщение об ошибке под полем "Телефон" красным цветом: "Неверный формат".
5. Заполнить поле "Электронная  почта" не валидными данными (Превышение длинны Email, адрес почты без знака @ , пробелы в имени и/или доменной части, отсутствие точки в доменной части, Email без имени или доменной части).
**Ожидаемый результат:** Появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

* Для авторизованного пользователя отсутствует поле "Электронная почта", поэтому тесты для проверки этого поля отсутствуют

### 2.Перечень используемых инструментов:

1. `IntelliJ IDEA`- интегрированная среда разработки ПО для многих языков программирования. Удобная среда подготовки авто-тестов.
2. `Java` - объектно-ориентированный язык программирования, оптимальный для написания понятных и наглядных автотестов.
3. `Gradle` - система автоматической сборки проектов, которая используется для упрощения работы с JAVA.
4. `JUnit5` - инструмент тестирования, среда модульного тестирования для языка программирования Java.
5. `Selenide` - это фреймворк для автоматизированного тестирования веб-приложений на основе Selenium WebDriver, дающий следующие преимущества: изящный API, поддержка AJAX для стабильных тестов, мощные селекторы, простая настройка.
6. `Faker` - это библиотека, которая позволяет генерировать случайные данные. С ее помощью можно заполнить таблицы в базе данных, построить корректные XML-документы, сформировать JSON-ответы для REST.
7. `REST Assured` - это фреймворк для тестирования API.
8. `Allure` - это система репортинга, для визуализации результатов проведения автотестов. Система проста в настройке и использовании в проекте.

### 3.Перечень необходимых разрешений/данных/доступов:

1. Техническая документация, чтобы опираться на валидные и невалидные данные, заложенные разработчиками. 
2. Разрешение на проведение тестирования веб-сайта [Нетология](https://netology.ru/)
3. Доступ к тестовой среде, если таковая имеется.
4. Доступ к БД.

### 4.Перечень и описание возможных рисков при автоматизации:

1. При изменении веб-элементов на странице, придется править автотесты.
2. Отсутствие технической документации.
3. Дополнительная нагрузка на сервер во время проведения тестов.
4. Запись в БД лишних неактуальных запросов.
5. Появление неактуальных заявок для обработки в отделе продаж.


### 5.Перечень необходимых специалистов для автоматизации:

Данная задача подойдет для выполнения junior-специалисту по автоматизированному тестированию, знакомому с перечисленными выше инструментами.

### 6.Интервальная оценка с учетом рисков в часах:

Для реализации данной задачи по автоматизации ориентировочно потребуется 25-30 рабочих часов.