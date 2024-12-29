# Запити зацікавлених осіб

## Вступ

Система управління відкритими даними дозволяє створювати, зберігати, оновлювати та шукати інформацію в базах даних, забезпечуючи контроль доступу до даних. Через складність цих процесів документ "Запити зацікавлених сторін" необхідний для того, щоб учасники проєкту мали чітке уявлення про те, як ці процеси функціонують у рамках системи.

### Мета

Метою цього документа є сформувати загальне розуміння продукту; проаналізувати основні бізнес-процеси, які відбуваються в системі, а також визначити учасників цих процесів та їхні права доступу; провести оцінку продукту, зосередившись на його перевагах і недоліках, використовуючи різноманітні критерії.

### Контекст

Цей документ пов'язаний із проєктами, що спрямовані на створення та розвиток платформ для зберігання, обробки та надання відкритих даних громадськості й бізнесу. Він впливає на впровадження систем управління даними, які забезпечують доступність, прозорість та ефективне використання відкритих даних, що можуть бути використані для аналітики, наукових досліджень, державного управління та розвитку нових цифрових продуктів і послуг.


### Основні визначення та скорочення

[Дані](https://uk.wikipedia.org/wiki/%D0%94%D0%B0%D0%BD%D1%96) (Data) — це сукупність фактів, цифр або інших інформаційних одиниць, які можуть бути використані для аналізу, прийняття рішень або побудови моделей. Дані можуть бути зібрані у вигляді числових значень, текстів, зображень або інших форм і зазвичай використовуються для отримання інформації або висновків через обробку або аналіз.

[Таблиця](https://uk.wikipedia.org/wiki/%D0%A2%D0%B0%D0%B1%D0%BB%D0%B8%D1%86%D1%8F_(%D0%B1%D0%B0%D0%B7%D0%B8_%D0%B4%D0%B0%D0%BD%D0%B8%D1%85)) (Table) — це базовий елемент структури бази даних, який організовує дані у вигляді рядків і стовпців. Кожен рядок представляє запис, а кожен стовпець — певний атрибут або властивість цих записів. Таблиці є основою для зберігання даних у реляційних базах і дозволяють організувати інформацію в структурованому вигляді.

[Запит](https://www.kievoit.ippo.kubg.edu.ua/kievoit/2012/25/25.html) (Query)  — це інструкція, надіслана до бази даних з метою отримання конкретної інформації. Запити формулюються за допомогою спеціальних мов програмування, таких як SQL (Structured Query Language), і можуть включати фільтри, сортування та інші умови для витягу потрібних даних з бази. Наприклад, SQL-запит може виглядати так: SELECT * FROM таблиця WHERE умова.

[CSV](https://uk.wikipedia.org/wiki/CSV) (Comma Separated Values) — це простий текстовий формат файлу, який використовується для зберігання табличних даних, де значення кожного рядка розділяються комами. CSV є одним з найбільш поширених форматів для зберігання відкритих даних, оскільки його можна легко читати та імпортувати в різні програми, зокрема електронні таблиці (наприклад, Excel).

[JSON](https://uk.wikipedia.org/wiki/JSON) (JavaScript Object Notation) — це легкий формат для обміну даними, який базується на тексті та використовується для зберігання і передачі структурованих даних, особливо між веб-сервісами та клієнтськими додатками. JSON широко використовується для передачі даних у веб-запитах і відповідає стандартам відкритих даних через його простоту і зручність у використанні.

[SQL](https://uk.wikipedia.org/wiki/SQL) (Structured Query Language)  — це мова структурованих запитів, яка використовується для управління і маніпуляції даними в реляційних базах даних. SQL дозволяє користувачам створювати, читати, оновлювати і видаляти записи у базі даних за допомогою спеціальних команд. Наприклад, за допомогою SQL можна вибирати конкретні дані з таблиці, фільтрувати їх за умовами або об'єднувати кілька таблиць для отримання комплексних результатів.

[NoSQL](https://uk.wikipedia.org/wiki/NoSQL) (Not Only SQL) – це тип баз даних, які призначені для зберігання та управління великими обсягами неструктурованих або слабо структурованих даних. На відміну від традиційних реляційних баз даних, які використовують таблиці з фіксованими полями для зберігання даних, NoSQL бази підтримують гнучкіші моделі зберігання. Вони зручні для великих і швидкозмінних даних (наприклад, дані соціальних мереж, інтернет-логів, або великих інтернет-магазинів).

[Великий обсяг даних](https://uk.wikipedia.org/wiki/%D0%92%D0%B5%D0%BB%D0%B8%D0%BA%D1%96_%D0%B4%D0%B0%D0%BD%D1%96) (Big Data) — це термін, який описує величезні набори даних, що характеризуються трьома основними ознаками: великим обсягом, високою швидкістю створення та великою різноманітністю. Ці дані часто надходять у нерегулярній формі (незалишкові), з багатьох джерел і в різних форматах (текстові файли, мультимедіа, лог-файли). Обробка таких даних вимагає використання спеціалізованих методів та інструментів (наприклад, Hadoop, Spark), оскільки традиційні бази даних і програми не здатні ефективно обробляти настільки великі та складні обсяги інформації.

[Стандартизація даних](https://profisee.com/blog/what-is-data-standardization) (Data Standardization) — це процес приведення даних до єдиного формату, який дозволяє зробити їх узгодженими і легкими для порівняння або аналізу. Це особливо важливо, коли дані збираються з різних джерел, де можуть використовуватися різні формати або одиниці виміру. Наприклад, стандартизація може включати перетворення дат в єдиний формат або приведення грошових одиниць до одного курсу валют. Стандартизація забезпечує сумісність даних і підвищує точність аналізу.

[Анонімізація даних](https://en.wikipedia.org/wiki/Data_anonymization) (Data Anonymization) — це процес, при якому особисті дані або інші ідентифікуючі атрибути видаляються або шифруються, щоб запобігти можливості ідентифікації окремих осіб або об'єктів. Це важливо для захисту конфіденційності користувачів при роботі з великими обсягами інформації, особливо у сфері охорони здоров'я, соціальних послуг або фінансів, де персональні дані є чутливими.

[Візуалізація даних](https://en.wikipedia.org/wiki/Data_and_information_visualization) (Data Visualization) — це метод представлення числових або текстових даних у графічних формах, таких як діаграми, графіки або інтерактивні карти. Основна мета візуалізації — полегшити розуміння великих наборів даних, виділяючи ключові закономірності або тренди, які можуть бути важко помітити в сирих числових таблицях. Візуалізація особливо важлива у випадках, коли дані складні або мають велику кількість змінних, таких як економічні показники або статистика охорони здоров'я.



### Посилання

1. [Дані](https://uk.wikipedia.org/wiki/%D0%94%D0%B0%D0%BD%D1%96)
2. [Таблиця](https://uk.wikipedia.org/wiki/%D0%A2%D0%B0%D0%B1%D0%BB%D0%B8%D1%86%D1%8F_(%D0%B1%D0%B0%D0%B7%D0%B8_%D0%B4%D0%B0%D0%BD%D0%B8%D1%85))
3. [Запит](https://www.kievoit.ippo.kubg.edu.ua/kievoit/2012/25/25.html)
4. [CSV](https://uk.wikipedia.org/wiki/CSV)
5. [JSON](https://uk.wikipedia.org/wiki/JSON)
6. [SQL](https://uk.wikipedia.org/wiki/SQL)
7. [NoSQL](https://uk.wikipedia.org/wiki/NoSQL)
8. [Великий обсяг даних](https://uk.wikipedia.org/wiki/%D0%92%D0%B5%D0%BB%D0%B8%D0%BA%D1%96_%D0%B4%D0%B0%D0%BD%D1%96)
9. [Стандартизація даних](https://profisee.com/blog/what-is-data-standardization)
10. [Анонімізація даних](https://en.wikipedia.org/wiki/Data_anonymization)
11. [Візуалізація даних](https://en.wikipedia.org/wiki/Data_and_information_visualization)

## Короткий зміст

- [Характеристика ділових процесів](#processes)
 - [Користувач](#user)
  - [Створити обліковий запис](#create-account)
  - [Увійти в обліковий запис](#sign-in)
  - [Знайти дані](#find-data)
  - [Завантажити дані](#download-data)
  - [Відправити відгук](#send-feedback)
 - [Адміністратор](#admin)
  - [Змінити список джерел даних](#change-sources-list)
  - [Редагувати дані](#edit-data)
  - [Додати категорію користувачів](#create-user-cat)
  - [Змінити права групи користувачів](#change-user-cat-rights)
  - [Змінити належність конкретного користувача до категорій](#change-cat-for-user)
  - [Видалити категорію користувачів](#delete-user-cat)
 - [Суперадміністратор](#superadmin)
  - [Додати адміністратора](#add-admin)
  - [Зняти права адміністратора](#un-admin)
- [Короткий огляд продукту](#descr)
 - [Функціональність](#functionality)
  - [Функції, доступні користувачам](#user-func)
  - [Функції, доступні адміністраторам](#admin-func)
 - [Практичність](#usability)
 - [Надійність](#reliability)
 - [Продуктивність](#performance)
 - [Експлуатаційна придатність](#supportability)

## <a id="processes">Характеристика ділових процесів</a>

### <span id="user">Користувач</span>

ID: | <span id="create-account">CreateAccount</span>
---|---
НАЗВА: | Створити обліковий запис
УЧАСНИКИ: | Користувач, Система
ПЕРЕДУМОВИ: | Відсутність облікового запису
РЕЗУЛЬТАТ: | Обліковий запис
ВИКЛЮЧНІ СИТУАЦІЇ: | Мінімум 1 обов'язкове поле порожне - EmptyRequiredField<br>Неправильна адреса електронної пошти - InvalidEmail<br>Пароль не відповідає вимогам - WeakPassword<br>Адреса електронної пошти вже використовується в іншому обліковому записі - EmailAlreadyInUse<br>Неправильний код підтвердження - InvalidVerificationCode
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Користувач натискає кнопку "Реєстрація".<br>2. Користувач вводить дані.<br>3. Користувач натискає кнопку "Зареєструватися".(можливі винятки EmptyRequiredField, InvalidEmail, WeakPassword)<br>4. Система перевіряє наявність облікового запису з введеною адресою електронної пошти.(можливий виняток EmailAlreadyInUse)<br>5. Система надсилає лист з кодом підтвердження на введену адресу електронної пошти.<br>6. Користувач вводить код підтвердження в поле.(можливий виняток EmptyRequiredField)<br>7. Користувач натискає кнопку "Підтвердити".<br>8. Система перевіряє введений код підтвердження.(можливий виняток InvalidVerificationCode)<br>9. Система створює обліковий запис.<br>10. Система повідомляє користувачу про створення облікового запису.

ID: | <span id="sign-in">SignIn</span>
---|---
НАЗВА: | Увійти в обліковий запис
УЧАСНИКИ: | Користувач, Система
ПЕРЕДУМОВИ: | Наявність облікового запису
РЕЗУЛЬТАТ: | Доступ до облікового запису
ВИКЛЮЧНІ СИТУАЦІЇ: | Мінімум 1 обов'язкове поле порожне - EmptyRequiredField<br>Неправильна адреса електронної пошти - InvalidEmail<br>Облікового запису не існує - AccountDoNotExist<br>Неправильний пароль - InvalidPassword
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Користувач натискає кнопку "Вхід".<br>2. Користувач вводить дані облікового запису.<br>3. Користувач натискає кнопку "Увійти".(можливі винятки EmptyRequiredField, InvalidEmail)<br>4. Система перевіряє дані.(можливі винятки AccountDoNotExist, InvalidPassword)<br>5. Система надає користувачу доступ до облікового запису.<br>6. Система повідомляє користувачу про вхід в обліковий запис.

ID: | <span id="find-data">FindData</span>
---|---
НАЗВА: | Знайти дані
УЧАСНИКИ: | Користувач, Система
ПЕРЕДУМОВИ: | Наявність доступу до облікового запису
РЕЗУЛЬТАТ: | Знайдені дані
ВИКЛЮЧНІ СИТУАЦІЇ: | Дані, які відповідають критеріям, відсутні або недоступні - DataDidNotFound
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Користувач натискає кнопку "Пошук".<br>2. Користувач вказує критерії пошуку.<br>3. Користувач натискає кнопку "Знайти".<br>4. Система здійснює пошук.(можливий виняток DataDidNotFound)<br>5. Система відправляє знайдені дані користувачу.

ID: | <span id="download-data">DownloadData</span>
---|---
НАЗВА: | Завантажити дані
УЧАСНИКИ: | Користувач, Система
ПЕРЕДУМОВИ: | Знайдені дані
РЕЗУЛЬТАТ: | Файл з даними
ВИКЛЮЧНІ СИТУАЦІЇ: | Помилка створення файлу - CreateFileError<br>Помилка завантаження - DownloadError
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Користувач обирає дані, які потрібно завантажити.<br>2. Користувач натискає кнопку "Завантажити".<br>3. Користувач обирає формат файлу.(можливий виняток CreateFileError)<br>4. Система створює файл з даними.(можливий виняток DownloadError)<br>5. Система відправляє створений файл з даними на пристрій користувача.<br>6. Система повідомляє користувачу про завантаження файлу.

ID: | <span id="send-feedback">SendFeedback</span>
---|---
НАЗВА: | Відправити відгук
УЧАСНИКИ: | Користувач, Система
ПЕРЕДУМОВИ: | Знайдені дані
РЕЗУЛЬТАТ: | Відправлений відгук
ВИКЛЮЧНІ СИТУАЦІЇ: | Поле порожне - EmptyField
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Користувач обирає дані, щодо яких потрібно залишити відгук.<br>2. Користувач натискає кнопку "Відгук".<br>3. Користувач вводить відгук.<br>4. Користувач натискає кнопку "Відправити".(можливий виняток EmptyField)<br>5. Система отримує відправлений відгук.<br>6. Система повідомляє користувача про отримання відгуку.

### <span id="admin">Адміністратор</span>

ID: | <span id="change-sources-list">ChangeSourcesList</span>
---|---
НАЗВА: | Змінити список джерел даних
УЧАСНИКИ: | Адміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Змінений список джерел даних
ВИКЛЮЧНІ СИТУАЦІЇ: | Неправильний формат запису джерела - InvalidSourceFormat
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Адміністратор натискає кнопку "Змінити список джерел" в меню "Адміністратор".<br>2. Система відправляє список джерел даних.<br>3. Адміністратор змінює список джерел даних(додає/редагує/видаляє джерела).<br>4. Адміністратор натискає кнопку "Зберегти".(можливий виняток InvalidSourceFormat)<br>5. Система зберігає змінений список джерел даних.<br>6. Система повідомляє адміністратора про зміну списку джерел даних.

ID: | <span id="edit-data">EditData</span>
---|---
НАЗВА: | Редагувати дані
УЧАСНИКИ: | Адміністратор, Система
ПЕРЕДУМОВИ: | Знайдені дані
РЕЗУЛЬТАТ: | Відредаговані дані
ВИКЛЮЧНІ СИТУАЦІЇ: | Неправильний формат запису даних - InvalidDataFormat<br>Мінімум 1 обов'язкове поле порожне - EmptyRequiredField
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Адміністратор обирає дані, які потрібно відредагувати.<br>2. Адміністратор натискає кнопку "Редагувати".<br>3. Адміністратор редагує дані.<br>4. Адміністратор натискає кнопку "Зберегти".(можливий виняток InvalidDataFormat, EmptyRequiredField)<br>5. Система зберігає відредаговані дані.<br>6. Система повідомляє адміністратора про отримання відредагованих даних.

ID: | <span id="create-user-cat">CreateUserCat</span>
---|---
НАЗВА: | Додати категорію користувачів
УЧАСНИКИ: | Адміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Категорія користувачів
ВИКЛЮЧНІ СИТУАЦІЇ: | Категорія з такою назвою вже існує - CatNameAlreadyInUse
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Адміністратор натискає кнопку "Категорії користувачів" в меню "Адміністратор".<br>2. Адміністратор натискає кнопку "Створити".<br>3. Адміністратор обирає батьківську категорію.<br>4. Адміністратор вводить назву.<br>5. Адміністратор натискає кнопку "Створити".<br>6. Система перевіряє назву.(можливий виняток CatNameAlreadyInUse)<br>7. Система створює категорію користувачів.<br>8. Система повідомляє адміністратора про створення категорії користувачів.

ID: | <span id="change-user-cat-rights">ChangeUserCatRights</span>
---|---
НАЗВА: | Змінити права групи користувачів
УЧАСНИКИ: | Адміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Змінені права категорії користувачів
ВИКЛЮЧНІ СИТУАЦІЇ: | Немає
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Адміністратор натискає кнопку "Категорії користувачів" в меню "Адміністратор".<br>2. Адміністратор обирає категорію користувачів.<br>3. Адміністратор натискає кнопку "Змінити права".<br>3. Адміністратор змінює права категорії.<br>4. Адміністратор натискає кнопку "Зберегти".<br>5. Система зберігає права категорії.<br>7. Система повідомляє адміністратора про збереження прав категорії.

ID: | <span id="change-cat-for-user">ChangeCatForUser</span>
---|---
НАЗВА: | Змінити належність конкретного користувача до категорій
УЧАСНИКИ: | Адміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Змінена належність користувача до категорій
ВИКЛЮЧНІ СИТУАЦІЇ: | Такого користувача не існує - UserDoNotExist
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Адміністратор натискає кнопку "Зміна належності користувача до категорій" в меню "Адміністратор".<br>2. Адміністратор вводить дані облікового запису користувача.<br>3. Адміністратор натискає кнопку "Знайти".(можливий виняток UserDoNotExist)<br>4. Адміністратор змінює список категорій.<br>5. Адміністратор натискає кнопку "Зберегти".<br>6. Система зберігає змінені дані про належність користувача до категорій.<br>7. Система повідомляє адміністратора про збереження змін.

ID: | <span id="delete-user-cat">DeleteUserCat</span>
---|---
НАЗВА: | Видалити категорію користувачів
УЧАСНИКИ: | Адміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Категорія користувачів
ВИКЛЮЧНІ СИТУАЦІЇ: | Немає
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Адміністратор натискає кнопку "Категорії користувачів" в меню "Адміністратор".<br>2. Адміністратор обирає категорію користувачів.<br>3. Адміністратор натискає кнопку "Видалити".<br>4. Адмінстратор натискає кнопку "Підтвердити видалення".<br>5. Система видаляє категорію користувачів.<br>6. Система повідомляє адміністратора про видалення категорії користувачів.

### <span id="superadmin">Суперадміністратор</span>

ID: | <span id="add-admin">AddAdmin</span>
---|---
НАЗВА: | Додати адміністратора
УЧАСНИКИ: | Суперадміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Адміністратор
ВИКЛЮЧНІ СИТУАЦІЇ: | Такого користувача не існує - UserDoNotExist
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Суперадміністратор натискає кнопку "Адміністратори" в меню "Адміністратор".<br>2. Суперадміністратор натискає кнопку "Додати".<br>3. Суперадміністратор вводить дані облікового запису користувача.<br>4. Суперадміністратор натискає кнопку "Знайти".(можливий виняток UserDoNotExist)<br>5. Суперадміністратор натискає кнопку "Додати адміністратора".<br>6. Система додає користувача до списку адміністраторів.<br>7. Система повідомляє суперадміністратора про додання адміністратора.

ID: | <span id="un-admin">UnAdmin</span>
---|---
НАЗВА: | Зняти права адміністратора
УЧАСНИКИ: | Суперадміністратор, Система
ПЕРЕДУМОВИ: | Немає
РЕЗУЛЬТАТ: | Втрата адміністратором прав
ВИКЛЮЧНІ СИТУАЦІЇ: | Такого користувача не існує - UserDoNotExist
ОСНОВНИЙ СЦЕНАРІЙ: | 1. Суперадміністратор натискає кнопку "Адміністратори" в меню "Адміністратор".<br>2. Суперадміністратор обирає адміністратора.<br>4. Суперадміністратор натискає кнопку "Видалити".<br>5. Суперадміністратор натискає кнопку "Підтвердити видалення".<br>6. Система видаляє користувача із списку адміністраторів.<br>7. Система повідомляє суперадміністратора про зняття прав адміністратора.

## <a id="descr">Короткий огляд продукту</a>

Система управління відкритими даними (Open Data Management System) – це програмне забезпечення, яке забезпечує комплексні інструменти для збору, зберігання, обробки та публікації даних у відкритий доступ. Вона дозволяє організаціям ефективно керувати великими обсягами інформації з різних джерел, включаючи API, бази даних, та файли у різних форматах (CSV, JSON тощо). Система інтегрує можливості для стандартизації та очищення даних, що підвищує їх точність і якість. Крім того, вона підтримує автоматичне оновлення даних і дозволяє публікувати їх на публічних платформах або через веб-інтерфейси. Інструменти візуалізації, вбудовані в систему, дозволяють користувачам легко аналізувати дані через графіки, діаграми та інші візуальні форми. Завдяки гнучким налаштуванням прав доступу, система забезпечує безпечне зберігання конфіденційних даних, контролюючи доступ до них. Вона сприяє прозорості, підвищує відкритість урядових і комерційних даних, а також покращує взаємодію з інформацією для громадськості, дослідників та бізнесу.


## <span id="functionality">Функціональність</span>

### <span id="user-func">Функції, доступні користувачам:</span>

1. Пошук і перегляд даних – користувачі можуть шукати відкриті дані за категоріями, темами або ключовими словами і переглядати доступні набори даних.

2. Завантаження даних – можливість завантажувати обрані набори даних у різних форматах (CSV, JSON, XML) для подальшого аналізу або використання.

3. Фільтрація та сортування – користувачі можуть застосовувати різні фільтри до наборів даних, щоб вибирати лише ті дані, які відповідають їхнім критеріям, а також сортувати їх за різними показниками.

4. Візуалізація даних – доступ до вбудованих інструментів візуалізації, що дозволяють створювати графіки, діаграми та карти на основі вибраних даних.

5. API-доступ до даних – користувачі можуть отримувати дані через API для інтеграції з іншими програмами або аналітичними платформами.

6. Збереження запитів і результатів – можливість зберігати створені запити та результати для швидкого доступу або повторного використання в майбутньому.

7. Публікація відгуків – користувачі можуть залишати відгуки або коментарі про якість даних або вказувати на помилки для покращення наборів даних.


### <span id="admin-func">Функції, доступні адміністраторам:</span>

1. Управління джерелами даних – адміністратори можуть додавати, змінювати або видаляти джерела даних, а також налаштовувати автоматичне оновлення інформації з зовнішніх джерел (API, бази даних).

2. Очищення та стандартизація даних – можливість виконувати очистку даних від дублікатів, помилок та привести їх до єдиного стандарту перед публікацією.

3. Контроль прав доступу – адміністратори можуть налаштовувати рівні доступу для різних категорій користувачів, обмежувати доступ до конфіденційних даних або надавати права лише на перегляд певних даних.

4. Моніторинг використання даних – відстеження активності користувачів, запитів до даних і API, а також створення звітів про використання системи.

5. Управління публікацією даних – адміністратори можуть керувати публікацією нових наборів даних, редагувати або видаляти застарілі дані та налаштовувати періодичність їх оновлення.

6. Інтеграція з іншими системами – можливість налаштувати інтеграцію з іншими внутрішніми або зовнішніми системами через API або спеціалізовані модулі.

7. Безпека та аудит – адміністратори можуть контролювати безпеку системи, встановлювати політики щодо захисту даних і проводити аудит на предмет аномальної активності чи потенційних загроз.



## <span id="usability">Практичність</span>

1. Простота навігації

2. Зручний пошук та фільтрація

3. Швидкість завантаження та відгук системи

4. Можливість кастомізації

5. Візуалізація даних

6. Доступність для користувачів з обмеженими можливостями

7. Мультиплатформність і кросбраузерність



## <span id="reliability">Надійність</span>

1. Висока доступність

2. Автоматичне резервне копіювання

3. Стійкість до збоїв

4. Масштабованість

5. Контроль за станом системи

6. Журнали подій та аудит

7. Відмова від одного компонента без втрати доступу


## <span id="performance">Продуктивність</span>

1. Час відгуку системи

2. Обробка великих обсягів даних

3. Підтримка одночасних користувачів

4. Оптимізація запитів

5. Масштабованість під навантаженням

6. Kешування даних

7. Оптимізація роботи з великими наборами даних

## <span id="supportability">Експлуатаційна придатність</span>

1. Легкість оновлення

2. Модульність і розширюваність

3. Документованість

4. Моніторинг і сповіщення

5. Засоби діагностики та налагодження

6. Підтримка зворотної сумісності

7. Гнучкі налаштування підтримки