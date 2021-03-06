# TerminalLinux
## **Задание по терминалу Linux - [HW_Linux1.txt:](https://github.com/dinsafina/Linux_HW/blob/main/HW1_Linux.txt)**

---

### **_Задание №1 - Linux terminal (GitBash) commands_**

---

1) Посмотреть где я === `pwd`
2) Создать папку === `mkdir dir/`
3) Зайти в папку === `cd dir/`
4) Создать 3 папки === `mkdir dir1 dir2 dir3`
5) Зайти в любоую папку === `cd dir1/`
6) Создать 5 файлов (3 txt, 2 json) === `touch file1.txt file2.txt file3.txt list1.json list2.json`
7) Создать 3 папки === `mkdir com1 com2 com3`
8. Вывести список содержимого папки === `ls -la`
9) + Открыть любой txt файл === `nano file1.txt` 
10) + написать туда что-нибудь, любой текст. === `qwerty`
11) + сохранить и выйти. === `ctrl+s ctrl+x`
12) Выйти из папки на уровень выше === `cd ..`
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку. === `mv dir1/file1.txt dir2/; mv dir1/file2.txt  dir2/`

14) скопировать любые 2 файла, которые вы создали, в любую другую папку. === `cp dir1/list1.json dir2/; cp dir1/list2.json dir2/`
15) Найти файл по имени === `find /home/ayrat/ -name file3.txt`
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. === `tail -f lorem '/home/ayrat/Desktop/diro/dir1/com1/file1.txt'`
17) вывести несколько первых строк из текстового файла  === `head -n2 file1.txt`
18) вывести несколько последних строк из текстового файла === `tail -n2 file1.txt`
19) просмотреть содержимое длинного файла (команда less) изучите как она работает. === `less file1.txt`
20) вывести дату и время === `date`
=========

### **_*Задание №2 - Отправить http запрос на сервер._**
` curl http://162.55.220.72:5005/terminal-hw-request;
curl 'http://162.55.220.72:5005/get_method?name=Vikram&age=25'`

### **_*Задание №3 - Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13_**
`touch dz_Linux.sh
nano dz_Linux.sh`

#!/bin/bash
cd dir/
mkdir dir1 dir2 dir3
cd dir/
touch file1.txt file2.txt file3.txt list1.json list2.json
mkdir com1 com2 com3
ls -la
mv file1.txt file2.txt com1

Команда: `bash dz_Linux.sh`

## **Задание по GIT - [scenario_git.txt](https://github.com/dinsafina/Linux_HW/blob/main/scenario_git.txt)**

---
 1. Создайте текстовый файл как в первом ДЗ по Terminal.
 2. Сценарий перенесите в этот файл.
 3. Напротив каждого действия - напишите команду в GitBash
 
 **JSON**

 4. Создать внешний репозиторий c названием JSON. === `в github страница "Create a new repository"`
 
 5. Клонировать репозиторий JSON на локальный компьютер. === `git clone git@github.com:dinsafina/JSON.git`

6. Внутри локального JSON создать файл “new.json”. === `touch new.json`

7. Добавить файл под гит. === `git add new.json` 

8. Закоммитить файл. === `git commit -m "add new.json file"`

9. Отправить файл на внешний GitHub репозиторий. === `git push`

10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON. === `nano new.json; 
  { 
	"first_name": "Dinara",
        "last_name":"Safina",
        "age": 27,
        "pets": 0,
        "desired_salary": 60000
   }`
 
 11. Отправить изменения на внешний репозиторий. === `git add new.json; git commit -m "add information about user";  git push`

12. Создать файл preferences.json === `touch preferences.json`

13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON. === `nano preferences.json;    
 {
	"movie": "Titanic",
	"series" : "Lie to me",
	"food" : "sushi",
        "season" : "Spring",
	"favorite_country" : "Norway" 

   }`

 14. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON === `touch skills.json; nano skills.json ; список скиллов`
 15. Отправить сразу 2 файла на внешний репозиторий. === `git add . ; git commit -m "add preferences.json and skills.json files"; git push`
 16. На веб интерфейсе создать файл bug_report.json. === `Add file -> create new file`
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе. === `commit new file`
 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON. ===
 `{
  "summary": "At the bottom of the Contacts page, a Google map is displayed
not completely",
  "project" : "site example.com",
  "version" : 1.0 ,
  "priority" : "medium",
  "severity" : "major",
  "status" : "new" ,
  "author": "Safina_Dinara",
  "assigned_to": "test coordinator",
  "result" : "Google map is not fully displayed on the site",
  "expected_result" : "Google map is fully displayed on the site"
 }`
 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе. 
 20. Синхронизировать внешний и локальный репозиторий JSON === `git pull`
 
 
 **XML**
 21. Создать внешний репозиторий c названием XML. === `в github страница "Create a new repository"`
 22. Клонировать репозиторий XML на локальный компьютер. === `git clone git@github.com:dinsafina/XML.git`
 23. Внутри локального XML создать файл “new.xml”. === `touch new.xml`
 24. Добавить файл под гит. === `git add new.xml `
 25. Закоммитить файл. === `git commit -m "add new.xml file"`
 26. Отправить файл на внешний GitHub репозиторий. === `git push`
 27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML. === `nano new.xml;
  <?xml version ="1.0"?>
  <user>
   <first_name>Dinara</first_name>
   <last_name>Safina</last_name>
   <age>27</age> 
   <pets>0</pets>
   <salary>60000</salary>
  </user>`

 28. Отправить изменения на внешний репозиторий. === `git add new.xml; git commit -m "add information about user"; git push`
 29. Создать файл preferences.xml === `touch preferences.xml`
 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML. ===` nano preferences.xml; 
 <?xml version="1.0"?>
  <preferences>
   <movie>Titanic</movie>
   <series>Lie_to_me</series>
   <food>sushi</food> 
   <season>Spring</season>
   <country>Norway</country>
  </preferences>`
  
 31. Создать файл skills.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML === `touch skills.xml; nano skills.xml;
<?xml version ="1.0"?>
  <skills>
   <one>Базовая теория</one>
   <two>Мобильное тестирование</two>
   <three>Основы_SQL</three> 
   <four>Доступ к удаленным серверам</four>
   <five>Работа с Postman</five>
  </skills>`

 32. Сделать коммит в одну строку. === `git add . | git commit -a "add skills.xml file"`
 33. Отправить сразу 2 файла на внешний репозиторий. === `git push`
 34. На веб интерфейсе создать файл bug_report.xml. === `Add file -> create new file`
 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе. === `Commit new file`
 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML. === 
 
 `<?xml version ="1.0"?>
 <bug_report>
   <summary>At the bottom of the Contacts page, a Google map is displayed not completely</summary>
   <project>site example.com</project>
   <version>1.0</version>
   <priority>medium</priority>
   <severity>major</severity> 
   <status>new</status>
   <author>Safina_Dinara</author>
   <assigned_to>test coordinator</assigned_to>
   <result>Google map is not fully displayed on the site</result>
   <expected_result>Google map is fully displayed on the site</expected_result>
 </bug_report>`
 
 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 38. Синхронизировать внешний и локальный репозиторий XML ===  `git pull`
 
 
**TXT**
 1. Создать внешний репозиторий c названием TXT. === `в github страница "Create a new repository"`
 2. Клонировать репозиторий TXT на локальный компьютер. === `git clone git@github.com:dinsafina/TXT.git`
 3. Внутри локального TXT создать файл “new.txt”. === `touch new.txt`
 4. Добавить файл под гит. === `git add new.txt`
 5. Закоммитить файл. === `git commit -m "Add new.txt file"`
 6. Отправить файл на внешний GitHub репозиторий. === `git push`
 7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT. ===
 
 `Сафина Динара Ильдаровна
Возраст: 27 лет
Домашние животные: нет
Желаемая зарплата: 50.000 руб`

 8. Отправить изменения на внешний репозиторий. === `git add new.txt; git commit -m "add information about user"; git push`
 9. Создать файл preferences.txt === `touch preferences`
 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT. ===

`Любимый фильм: "Титаник"
Любимый сериал: "Обмани меня"
Любимая еда: Борщ
Любимое время года: Весна
Страна, которую хотели бы посетить: Норвегия`

 11. Создать файл skills.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT === `touch skills.txt
 
1. Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC.
2. Что такое клиент-серверная архитектура.
3. HTTP Методы запросов на сервер.
4. Коды ответов HTTP сервера.
5. Структуры HTTP запросов и ответов.
6. Что такое JSON, XML. Их структура.`

 12. Сделать коммит в одну строку. === `git add . | git commit -a "add skills.txt file"`
 13. Отправить сразу 2 файла на внешний репозиторий. === `git push`
 14. На веб интерфейсе создать файл bug_report.txt. === `Add file -> create new file`
 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе. 
 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT. === 

`summary: At the bottom of the Contacts page, a Google map is displayed not completely,
project : site example.com,
version : 1.0,
priority : medium,
severity :major,
status : new,
author: Safina_Dinara,
assigned_to: test coordinator,
result : Google map is not fully displayed on the site,
expected_result : Google map is fully displayed on the site`
 
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе. 
 18. Синхронизировать внешний и локальный репозиторий TXT === `git pull`


## **Задание по GitHub**
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

2. Запушить все ветки на внешний репозиторий
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
4. Запушить структуру багрепорта на внешний репозиторий
5. Вмержить ветку Bag Reports в Main
6. Запушить main на внешний репозиторий.
7. В ветке CheckLists набросать структуру чек листа.
8. Запушить структуру на внешний репозиторий
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main

