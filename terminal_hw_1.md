1) Посмотреть где я	pwd
2) Создать папку		mkdir Folder
3) Зайти в папку		cd Folder
4) Создать 3 папки	mkdir subfolder1 subfolder2 subfolder3
5) Зайти в любую папку	cd subfolder1	
6) Создать 5 файлов (3 txt, 2 json)		touch file1.txt file2.txt file3.txt file4.json file5.json
7) Создать 3 папки	mkdir lk1 lk2 lk3
8. Вывести список содержимого папки		ls -la
9) + Открыть любой txt файл		vim file1.txt
10) + написать туда что-нибудь, любой текст. 	
Hello
Alena
Alex
Vlad
Marina
Sergey
Vova
Tania
Larisa
11) + сохранить и выйти.	esc. :wq
12) Выйти из папки на уровень выше		cd ..
13) переместить любые 2 файла, которые вы создали, в любую другую папку. 	mv subfolder1/file1.txt subfolder1/file2.txt subfolder2	
14) скопировать любые 2 файла, которые вы создали, в любую другую папку.	cp subfolder1/file3.txt subfolder1/file5.json subfolder3 
15) Найти файл по имени		find . -name “file1.txt”					
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.	tail -f ./subfolder2/file1.txt | grep "Hello"
17) вывести несколько первых строк из текстового файла	head -3 ./subfolder2/file1.txt
18) вывести несколько последних строк из текстового файла		tail -3 ./subfolder2/file1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает.	less ./subfolder2/file1.txt
20) вывести дату и время		date
=========

Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request		

Last login: Sun Apr 16 15:15:43 on ttys000
alena@Air-vlad ~ % curl http://162.55.220.72:5005/terminal-hw-request

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">
<title>404 Not Found</title>
<h1>Not Found</h1>
<p>The requested URL was not found on the server. If you entered the URL manually please check your spelling and try again.</p>
alena@Air-vlad ~ % 

Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

#!/bin/bush
cd Folder
mkdir subfolder1 subfolder2 subfolder3
cd subfolder1
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir lk1 lk2 lk3
ls -la
mv file1.txt file2.txt ../subfolder2
