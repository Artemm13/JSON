1. Создать внешний репозиторий c названием JSON.
В GitHub нажимаем "New" --> в "Repository name" пишем JSON и нажимаем кнопку "Create repository".

 2. Клонировать репозиторий JSON на локальный компьютер.
 Через терминал заходим в необходимую папку на компе: cd QA/GIT (/Users/artemm/QA/GIT). Пишем в терминале команду: git clone и вставляем ссылку из GitHub: https://github.com/Artemm13/JSON.git

 3. Внутри локального JSON создать файл “new.json”.
 В терминале пишем команду: touch new.json

 4. Добавить файл под гит.
 В терминале пишем команду: git add .

 5. Закоммитить файл.
 В терминале пишем команду: git commit -m "Commit json"

 6. Отправить файл на внешний GitHub репозиторий.
 В терминале пишем команду: git push

 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
 Пишем команду: vim new.json В открывшемся редакторе нажимаем клавишу "i" и пишем текст: 
{
  "name": "Mishchenko Artem",
  "age": 37,
  "pets": 1,
  "future_salary": 4000
}
Переходим в нормальный режим (клавиша "esc"), сохраняем - :w, и выходим - :q.


 8. Отправить изменения на внешний репозиторий.
 Пишем: git add . 
        git commit -m "Changes json" 
        git push

 9. Создать файл preferences.json
 Пишем команду: touch preferences.json

 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
 Пишем команду: vim preferences.json и пишем текст редакторе:
{
  "favorite_movie": "Matrix",
  "favorite_show": "Friends",
  "favorite_food": "kebab",
  "favorite_time_of_year": "Autumn",
  "country_you_would_like_to_visit": "Netherlands"
}

 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
 Пишем команды: touch skills.json
                vim skills.json
{
  "skills": [

    "Linux terminal",
    "GitHub",
    "Postman",
    "SQL",
    "DevTools",
    "Mobile testing",
    "Fidler and Charles"
 ]  
}

 13. Отправить сразу 2 файла на внешний репозиторий.
 Пишем команды: git add preferences.json skills.json
                git commit -m "Commit preferences.json and skills.json"
                git push

 14. На веб интерфейсе создать файл bug_report.json. 
 В GitHab нажимаем "Add file" --> "Create new file" --> пишем название файла "bug_report.json"

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Нажимаем кнопку "Commit changes" --> при необходимости заполняем поле "Extended description" и нажимаем "Commit changes".

 16. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
 Открываем файл "bug_report.json" --> выбираем иконку "Edit this file" --> пишем баг репорт:
{
  "id": 111,
  "summary": "The filter is not reset when the 'Filter reset' button is pressed",
  "steps": [

    "1. Go to exe.ua",
    "2. In the catalog, select the category 'PC components', 'Video cards'",
    "3. Filtering goods by 'graphic chip'. Choose from the list RTX 3060 Ti",
    "4. Press the 'Filter products' button",
    "5. Press the 'Filter reset' button",
  ]
  "expected_result": "The filter is reset",
  "actual_result": "The filter is not reset",
  "severity": "Low",
  "priority": "Medium",
  "type": "Functional",
  "assigned": "Artem M",
  "state": "Open",
  "date_of_creation": "01-11-2022",
  "environment": "Windows 10, Chrome 106.0.5249.119",
  "attachment": "https://...",
}

 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Нажимаем кнопку "Commit changes" --> при необходимости заполняем поле "Extended description" и нажимаем "Commit changes".

 17. Синхронизировать внешний и локальный репозиторий JSON
 Пишем в терминале команду: git pull origin main
