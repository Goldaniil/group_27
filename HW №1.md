[[qa]]

1) Посмотреть где я

1.  daniilgolubev@MBP-Daniil Terminal % pwd

/Users/daniilgolubev/Downloads/QA/Terminal

2) Создать папку

daniilgolubev@MBP-Daniil Terminal % mkdir folder

3) Зайти в папку

daniilgolubev@MBP-Daniil Terminal % cd folder

4) Создать 3 папки

1.  daniilgolubev@MBP-Daniil folder % mkdir folder{1,2,3} 

5) Зайти в любоую папку

1.  daniilgolubev@MBP-Daniil folder % cd folder1

6) Создать 5 файлов (3 txt, 2 json)

1.  daniilgolubev@MBP-Daniil folder1 % touch file{1,2,3}.txt jile{1,2}.json

7) Создать 3 папки

1.  daniilgolubev@MBP-Daniil folder1 % mkdir folder{a,b,c}

8. Вывести список содержимого папки

1.  daniilgolubev@MBP-Daniil folder1 % ls
2.  file1.txt file3.txt folderb jile1.json
3.  file2.txt foldera folderc jile2.json

9) + Открыть любой txt файл

1.  daniilgolubev@MBP-Daniil folder1 % nano file1.txt

10) + написать туда что-нибудь, любой текст.

11) + сохранить и выйти.

:wq

12) Выйти из папки на уровень выше

1.  daniilgolubev@MBP-Daniil folder1 % cd ../

—

13) переместить любые 2 файла, которые вы создали, в любую другую папку.

1.  daniilgolubev@MBP-Daniil folder % mv ./folder1/file{1,2}.txt ./folder2

14) скопировать любые 2 файла, которые вы создали, в любую другую папку.

1.  cp ./folder1/jile{1,2}.json ./folder3 

15) Найти файл по имени

1.  daniilgolubev@MBP-Daniil folder % find ./ -name "file?.txt"

16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.

tail -f filename

17) вывести несколько первых строк из текстового файла

head -2 filename

18) вывести несколько последних строк из текстового файла

tail -2 filename

19) просмотреть содержимое длинного файла (команда less) изучите как она работает.

less filename

20) вывести дату и время

date

=========

  

Задание *

1) Отправить http запрос на сервер.

http://162.55.220.72:5005/terminal-hw-request

$ curl http://162.55.220.72:5005/terminal-hw-request

 % Total % Received % Xferd Average Speed Time Time Time Current

 Dload Upload Total Spent Left Speed

100 237 100 237 0 0 2943 0 --:--:-- --:--:-- --:--:-- 3000{"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}

  

$ curl "http://162.55.220.72:5005/get_method?name=Daniil&age=28"

 % Total % Received % Xferd Average Speed Time Time Time Current

 Dload Upload Total Spent Left Speed

100 16 100 16 0 0 201 0 --:--:-- --:--:-- --:--:-- 205["Daniil","28"]

  

.2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

  

  

1.  cp ./folder1/jile{1,2}.json ./folder3 
2.  daniilgolubev@MBP-Daniil folder % find ./ -name "file?.txt"
3.  .//folder2/file2.txt
4.  .//folder2/file1.txt
5.  .//folder1/file3.txt