ЗАДАНИЕ 1
1. Посмотреть где я
pwd
2. Создать папку
mkdir Terminal
3. Зайти в папку
cd Terminal
4. Создать 3 паки
mkdir d1 d2 d3
5. Зайти в любую папку
cd d1
6. Создать 5 файлов (3 txt, 2 json)
touch f1.txt f2.txt f3.txt f4.json f5.json
7. Создать 3 папки
mkdir dir_1 dir_2 dir_3
8. Вывести список содержимого папки
ls -la
9. Открыть любой txt файл
vim f1.txt
10. Написать туда что-нибудь, любой текст
I love to study. 
I am studing linux terminal.
11. Сохранить и выйти
#esc + :wq + enter
12. Выйти из папки на уровень выше
cd ..
13. Переместить любые 2 файла, которые создали, в любую другую папку
mv f1.txt f2.txt ../dir_1
14. Переместить любые 2 файла, которые создали, в любую другую папку
cp f3.txt f4.json f5.json ../dir_1
15. Найти файл по имени
find -name f3
16. Просмотреть содержимое в реальном времени
tail -f f1.txt
17. Вывести несколько первых строк из текстового файла
head -5 f1.txt
18. Вывести несколько последних строк из текстового файла
tail -n5 f1.txt
19. Просмотреть содержимое длинного файла
less f1.txt Выход: q
20. Вывести дату и время
date

ЗАДАНИЕ 2
Отправить http запрос на сервер
curl http://162.55.220.72:5005/terminal-hw-request
приходит ответ с запросом имени и возраста отправляем:
curl http://162.55.220.72:5005/get_method?name="Vladimir"\&age=33

ЗАДАНИЕ 3
Написать скрипт, который выполнитавтоматически пункты 3, 4, 5, 6, 7, 8, 13
touch script_hw1.sh
vim script_hw1.sh
#!/bin/bash
cd terminal
mkdir d1 d2 d3
cd d1
touch f1.txt f2.txt f3.txt f4.json f5.json
mkdir dir_1 dir_2 dir_3
ls -la
mv f1.txt f2.txt ../dir_1
выйти и сохранить: нажимаем
esc :wq + enter
- запускаем
sh script_hw1.sh