## План тестирования возможности записи на обучение профессии ["Инженер по тестированию"](https://netology.ru/programs/qa-middle).

### 1.Перечень автоматизируемых сценариев:

### Предусловия:

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

### Тестовые сценарии:

#### Позитивные:

##### Пользователь не зарегистрирован или не авторизован на сайте

**№1.Успешная отправка заявки**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка успешно отправлена, на электронный адрес приходит письмо с подтверждением заявки.

##### Пользователь зарегистрирован и авторизован на сайте

**№1.Успешная отправка заявки**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка успешно отправлена, на зарегистрированный электронный адрес приходит письмо с подтверждением заявки.

#### Негативные:

##### Пользователь не зарегистрирован или не авторизован на сайте

**№1.Заполнение поля "Имя" спец.символами**
1. В поле "Имя" ввести спец.символы.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Имя" красным цветом: "Должно состоять из букв"

**№2.Заполнение поля "Имя" пробелами**
1. В поле "Имя" ввести пробелы.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Имя" красным цветом: "Обязательное поле"

**№3.Граничное значение поля "Имя" на кириллице**
1. В поле "Имя" ввести одну букву на кириллице.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Имя" красным цветом: "Должно быть не короче 2 символов"

**№4.Граничное значение поля "Имя" на латинице**
1. В поле "Имя" ввести одну букву на латинице.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Имя" красным цветом: "Должно быть не короче 2 символов"

**№5.Заполнение поля "Имя" цифрами**
1. В поле "Имя" ввести цифры.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Имя" красным цветом: "Должно состоять из букв"

**№6.Заполнение поля "Номер телефона" спец.символами**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести спец.символы.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Телефон" красным цветом: "Неверный формат".

**№7.Заполнение поля "Номер телефона" латинскими буквами**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести латинские буквы.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Телефон" красным цветом: "Неверный формат".

**№8.Заполнение поля "Номер телефона" кириллическими буквами**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести кириллические буквы.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Телефон" красным цветом: "Неверный формат".

**№9.Граничное значение поля "Номер телефона" из 10 цифр**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести 10 цифр.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Телефон" красным цветом: "Неверный формат".

**№10.Граничное значение поля "Номер телефона" из 12 цифр**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести 12 цифр.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Телефон" красным цветом: "Неверный формат".

**№11.Заполнение поля "Электронная почта" адресом без символа "@"**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести адрес электронной почты без символа "@".
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

**№12.Заполнение поля "Электронная почта" адресом с пробелом в имени**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести адрес электронной почты с пробелом в имени.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

**№13.Заполнение поля "Электронная почта" адресом с пробелом в доменной части**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99. 
3. В поле "Электронная почта" ввести адрес электронной почты с пробелом доменной части.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

**№14.Заполнение поля "Электронная почта" адресом без точки в доменной части**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99. 
3. В поле "Электронная почта" ввести адрес электронной почты без точки в доменной части.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

**№15.Заполнение поля "Электронная почта" адресом без имени**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99. 
3. В поле "Электронная почта" ввести адрес электронной почты без имени.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

**№16.Заполнение поля "Электронная почта" адресом без доменной части**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести адрес электронной почты без доменной части.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, появляется сообщение об ошибке под полем "Электронный адрес" красным цветом: "Неверный email".

**№17.Отправка формы с пустыми полями**
1. Поле "Имя" оставить пустым.
2. Поле "Номер телефона" оставить пустым.
3. Поле "Электронная почта" оставить пустым.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, каждое незаполненное поле подсвечивается красным цветом и появляется сообщение об ошибке под каждым незаполненным полем красным цветом: "Обязательное поле".

**№18.Отправка формы с пустым полем "Имя"**
1. Поле "Имя" оставить пустым.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, поле "Имя" подсвечивается красным цветом и появляется сообщение об ошибке под полем красным цветом: "Обязательное поле".

**№19.Отправка формы с пустым полем "Номер телефона"**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. Поле "Номер телефона" оставить пустым.
3. В поле "Электронная почта" ввести валидный адрес электронной почты.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, поле "Номер телефона" подсвечивается красным цветом и появляется сообщение об ошибке под полем красным цветом: "Обязательное поле".

**№20.Отправка формы с пустым полем "Электронная почта"**
1. В поле "Имя" ввести валидное значение имени: имя на латинице или кириллице не короче двух букв.
2. В поле с номером телефона ввести валидное значение для номера телефона: номер в формате +9 (999) 999-99-99.
3. Поле "Электронная почта" оставить пустым.
4. Нажать на кнопку `"Записаться"`.

**Ожидаемый результат:** Заявка не отправлена, поле "Электронная почта" подсвечивается красным цветом и появляется сообщение об ошибке под полем красным цветом: "Обязательное поле".

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