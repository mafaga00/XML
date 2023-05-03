# XML

 21. Создать внешний репозиторий c названием XML.     New
                                                      Create repository

 22. Клонировать репозиторий XML на локальный компьютер.   git clone git@github.com:AndreiHeranok/XML.git

 23. Внутри локального XML создать файл “new.xml”.  touch new.xml

 24. Добавить файл под гит.    git add . new.xml
 25. Закоммитить файл.       git commit -m "add xml"

 26. Отправить файл на внешний GitHub репозиторий.  git push
 
 27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.

Вносим изменения: vim new.xml
нажать клавишу "i" ввести текст

<info>
 <FIO>Heranok Andrei Vladimirovich</FIO>
 <AGE>29</AGE>
 <number_of_pets>1</number_of_pets>
 <Future_desired_salary>500</Future_desired_salary>
</info>

Cохранить и выйти: "esc" ":wq"

28. Отправить изменения на внешний репозиторий.   git commit -am "edit xml"
                                                  git push
 
29. Создать файл preferences.xml       touch preferences.xml

30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
  
Вносим изменения: vim preferences.xml
нажать клавишу "i" ввести текст

<Favorite>
 <Favorite_movie>The Big Lebowski</Favorite_movie>
 <Favorite_series>La casa de papel</Favorite_series>
 <favorite_food>Potato</favorite_food>
 <favorite_time_of_year>Summer</favorite_time_of_year>
 <country_you_like_to_visit>Canada</country_you_like_to_visit>
</Favorite>

Cохранить и выйти: "esc" ":wq"

 31. Создать файл skills.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML 

Создаём файл: touch skills.xml
Вносим изменения: vim skills.xml
нажать клавишу "i" ввести текст

<skills>
    <Базовая_теория>Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования, SDLC, STLC</Базовая_теория>,
    <клиент_сервер>клиент-серверная архитектура</клиент_сервер>,
    <Методы_запросов_на_сервер>HTTP<Методы_запросов_на_сервер>,
    <Коды_ответов>HTTP сервера</Коды_ответов>,
    <Структуры>HTTP запросов и ответов</Структуры>,
    <Структура>JSON, XML</Структуры>,
    <Тестирование_API>через Postman (JS, автотесты API)</Тестирование_API>,
    <Снятие_и_чтение_логов>c внешнего сервера</Снятие_и_чтение_логов>,
    <Снифинг>http web трафика через Charles и Fiddler</Снифинг>,
    <Dev_Tools_веб_браузеров>Google Chrome, FireFox</Dev_Tools_веб_браузеров>,
    <VPN>Как работает, зачем нужен, как использовать, варианты инструментов</VPN>,
    <тестирование>Мобильное</тестирование>,
    <гайдлайны>Особенность iOS, Android</гайдлайны>,
    <Сборка>iOS приложений на XCode</Сборка>,
    <Сборка>Androidприложений на Android Studio</Сборка>,
    <ADB>управление андройд девайсами</ADB>,
    <Настройка>прокси и vpn на iOS и Android</Настройка>,
    <Перехват_(сниффинг)_мобильного_трафика>через Charles и Fiddler на iOS и Android</Перехват_(сниффинг)_мобильного_трафика>,
    <Командная_строка_(terminal)_Linux>копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса</Командная_строка_(terminal)_Linux>,
    <Основы_bash_скриптинг>автоматизация рутинных задач на сервере</Основы_bash_скриптинг>,
    <Доступ>к удалённым серверам</Доступ>,
    <Основы_SQL>Create, Delete, Drop, Insert Into, Select, From, Where, Join</Основы_SQL>,
    <База_данных>Postgres, установка, настройка и использование</База_данных>,
    <Нереляционная_база_данных>Redis установка, настройка и использование</Нереляционная_база_данных>,
    <Нагрузочное_тестирование>Jmeter</Нагрузочное_тестирование>,
    <Методология_разработки>Scrum</Методология_разработки>,
    <Python>Изучение основ. Создание клиент серверного приложения</Python>
</skills>

Cохранить и выйти: "esc" ":wq"

 32. Сделать коммит в одну строку.                   git commit -ma "add new xml"

 33. Отправить сразу 2 файла на внешний репозиторий.
                                                     git add . 
                                                     git commit -m "edit new xml"
                                                     git push

 34. На веб интерфейсе создать файл bug_report.xml.  - Add file
							    - Create new file
							    - Commit new file
 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе. -edit this file
                                                                     в строке Commit changes пишем новый Commit
                                                                     Commit changes

 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.

"<bug>
    <ID>1</ID>,
    <Version>Windows 10</Version>,
    <Summary>Не отображаеться предупреждающие окно в приложении при деление на ноль</Summary>,
    <Req_id>22.3</Req_id>,
    <Steps>ткрыть приложение, Ввести число, Нажать кнопку '/', вссети другое число, нажать кнопку '='</Steps>,
    <Actual_result>в полле ввода число 0,предупреждающего окна нету</Actual_result>,
    <Expected_result>Появляется окно ошибки с текстом,'вы не можете делить на 0'</Expected_result>,
    <Severity>Minor</Severity>,
    <Priority>Low</Priority>,
    <Attachments>screenshot</Attachments>
</bug>"

 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.    в строке Commit changes пишем новый Commit
                                                                     Commit changes
 38. Синхронизировать внешний и локальный репозиторий XML   git pull
