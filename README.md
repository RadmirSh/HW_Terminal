# HW_Terminal

### 1. Посмотреть где я
~~~
pwd
~~~
### 2. Создать папку
~~~
mkdir step_1
~~~
### 3. Зайти в папку
~~~
cd step_1
~~~
### 4. Создать 3 папки
~~~
mkdir wert_1 wert_2 wert_3
~~~
### 5. Зайти в любую папку
~~~
cd wert_3
~~~
### 6. Создать 5 файлов (3 txt, 2 json)
~~~
touch asd1.txt asd2.txt asd3.txt edc1.json edc2.json
~~~
### 7. Создать 3 папки
~~~
mkdir wer4 wer5 wer6
~~~
### 8. Вывести список содержимого папки
~~~
ls –la
~~~
### 9. Открыть любой txt файл
~~~
cat asd1.txt
~~~

### 10. Написать туда что-нибудь, любой текст
~~~
cat >> asd1.txt
~~~
>Содержимое asd1.txt:
~~~
44444
44555
table
smile 
computer
dog cat
monitor443
Big
Burger
kldsjfkojfpodkssssssssssssssssffnmknkonipjpojp
~~~
### 11. Сохранить и выйти
~~~
Enter, Ctrl+C
~~~
### 12. Выйти из папки на уровень выше
~~~
cd ..
~~~
___
### 13. Переместить любые 2 файла, которые вы создали, в любую другую папку
~~~
mv {wert_3/asd1.txt,wert_3/asd2.txt} wert_1
~~~
### 14. Скопировать любые 2 файла, которые вы создали, в любую другую папку
~~~
cp {wert_3/edc1.json,wert_3/edc2.json} wert_2
~~~
### 15. Найти файл по имени
~~~
find –name ‘asd1.txt’
~~~
### 16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает
~~~
tail -f wert_1/asd1.txt
~~~
### 17. Вывести несколько первых строк из текстового файла
~~~
head -n 3 wert_1/asd1.txt
~~~
>Результат:
~~~
44444
44555
table
~~~
### 18. Вывести несколько последних строк из текстового файла
~~~
tail -n 4 wert_1/asd1.txt
~~~
>Результат:
~~~
Big
Burger
kldsjfkojfpodkssssssssssssssssffnmknkonipjpojp
~~~
### 19. Просмотреть содержимое длинного файла (команда less) изучите как она работает
~~~
less wert_1/asd1.txt
~~~
### 20. Вывести дату и время
~~~
date
~~~
___
## Задание *
### 1. Отправить http запрос на [сервер](http://162.55.220.72:5005/terminal-hw-request)
~~~
curl -i http://162.55.220.72:5005/terminal-hw-request
~~~
### 2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
> создаю файл my_script.sh:
~~~
nano my_script.sh  
~~~

> прописываю в my_script.sh следующие команды:
~~~
#!bin/bash
mkdir test5
cd test5
mkdir tim1 tim2 tim3
cd tim3
touch boss1.txt boss2.txt boss3.txt party1.json party2.json
mkdir wer7 wer8 wer9
mv {boss1.txt,boss2.txt} wer7
ls -la
~~~
> сохраняю, выхожу:
~~~
Ctrl+S, Ctrl+X
~~~
>команда для доступа:
~~~
chmod +x my_script.sh 
~~~
>исполнение скрипта:
~~~
nano my_script.sh
~~~ 
