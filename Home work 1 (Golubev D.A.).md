1) Посмотреть где я
`pwd`

2) Создать папку
`mkdir folder

3) Зайти в папку
`cd folder

4) Создать 3 папки
`mkdir folder{1,2,3} 

5) Зайти в любоую папку
`cd folder1`

6) Создать 5 файлов (3 txt, 2 json)
`touch file{1,2,3}.txt jile{1,2}.json

7) Создать 3 папки
`mkdir folder{a,b,c}

8. Вывести список содержимого папки
`ls

9) + Открыть любой txt файл
`nano file1.txt

10) + написать туда что-нибудь, любой текст.

11) + сохранить и выйти.
`:wq

12) Выйти из папки на уровень выше
`cd ../

—

13) переместить любые 2 файла, которые вы создали, в любую другую папку.
`mv ./folder1/file{1,2}.txt ./folder2

14) скопировать любые 2 файла, которые вы создали, в любую другую папку.
`cp ./folder1/jile{1,2}.json ./folder3 

15) Найти файл по имени
`find ./ -name "file?.txt"

16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.
`tail -f filename

17) вывести несколько первых строк из текстового файла
`head -2 filename

18) вывести несколько последних строк из текстового файла
`tail -2 filename

19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
`less filename

20) вывести дату и время
`date

=========

  

Задание *

1) Отправить http запрос на сервер.

http://162.55.220.72:5005/terminal-hw-request

```
$ curl http://162.55.220.72:5005/terminal-hw-request

% Total % Received % Xferd Average Speed Time Time Time Current

Dload Upload Total Spent Left Speed

100 237 100 237 0 0 2943 0 --:--:-- --:--:-- --:--:-- 3000{"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}

  

$ curl "http://162.55.220.72:5005/get_method?name=Daniil&age=28"

 % Total % Received % Xferd Average Speed Time Time Time Current

 Dload Upload Total Spent Left Speed

100 16 100 16 0 0 201 0 --:--:-- --:--:-- --:--:-- 205["Daniil","28"]
```  

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
```
cp ./folder1/jile{1,2}.json ./folder3 
daniilgolubev@MBP-Daniil folder % find ./ -name "file?.txt"
.//folder2/file2.txt
.//folder2/file1.txt
.//folder1/file3.txt
```