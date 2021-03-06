# Резултати от НОИ2 2017г.
В това [репозитори][github] съм качил скрипт, генериращ резултатите от НОИ2. За да работи
съм качил също тестовете, авторовите решения и решенията на участниците.

|Web страница    |CSV                     |Разширени резултати CSV                   |
|:--------------:|:----------------------:|:----------------------------------------:|
| [A](results/A) | [A.csv](results/A.csv) | [A-extended.csv](results/A-extended.csv) |
| [B](results/B) | [B.csv](results/B.csv) | [B-extended.csv](results/B-extended.csv) |
| [C](results/C) | [C.csv](results/C.csv) | [C-extended.csv](results/C-extended.csv) |
| [D](results/D) | [D.csv](results/D.csv) | [D-extended.csv](results/D-extended.csv) |
| [E](results/E) | [E.csv](results/E.csv) | [E-extended.csv](results/E-extended.csv) |

## Защо ?
Поради скорошни промени в закона (мисля, не съм адвокат, *don't quote me on
this*), всички участници трябва да попълваме декларации (или родителите ни ако не
сме пълнолетни), че сме (са) съгласни да се публикуват резултатите ни. Разбира се, да
се съберат толкова много декларации не е лесна работа и тъй като някои липсват,
не е публикувано официално класиране. 


## Как ?
За радост на [keleved.com][keleved] са публикувани тестовете и работите на 
участниците (поне на тези които са предали декларация). Оценяването на решения на
задачи по информатика се извършва изцяло автоматизирано - програмата се пуска
с всички тестови данни и ако даде правилен отговор, се присъждат точки. Сиреч,
за няколко часа един кадърен програмист (като мен, разбира се ;)) може да напише
програма, съставяща класиране. Огромни благодарности към Националната Комисия за
публикуването на тестовете, авторовите решения и най-вече работите на участниците -
без тях този проект щеше да е невъзможен

## Къде са имената ?
Решенията на участниците са подредени в папки с техните иницали. Макар и много
от тях да имат и файл `info.txt` или `info.docx` с името на състезателя при
някои този файл лисва, а където ги има тези файлове не следват някакъв строг 
формат. Това прави четенето им от компютър трудна задача. Ако на някого му се 
занимава, може да добави имена (ръчно или програматично). На мен ми се спи ...

## Колко точни са тези резултати ?
Тук е момента да спомена, че тези резултати не са идентични с тези на
Националната Комисия (това са хората, организиращи олимпиадата). Това се дължи
на няколко причини:
 * На част от участниците не са публикувани работите. Би трявбало да са малко, но
   все пак биха могли да разместят класирането.
 * Тестването е извършено на моята машина. Използвал съм удвоеното време на 
   авторовото решение за ограничение по време, но не съм сигурен какви са
   времената, използвани от Националната комисия. По принцип това е стандартна
   практика, която се прилага дори на Междунарадната олимпиада по информатика
   (IOI), но човек никога не знае.
 * Използвам по-нова версия на компилатора от тази на Националната Комисия.
   Макар и да съм конкретизирал c++ версия 2003 `-std=c++03` има разминавания,
   водещи до проблеми с компилацията и 0 точки. Ако някой има такъв проблем може
   да ми [пише][email] и ще се погрижа да коригирам резултатите му.

## Мога ли да го ползвам ?
Разбира се, затова съм го качил в Github. Само не се присмивайте твърде мн на
некъдърния ми код, бързах. За съжаление в момента скрипта работи само под линукс
и нямам намерение да подържам windows. За да работи скрипта ти трябват python 3+
и [isolate sandbox][isolate] - това е програма, която ограничава привилегиите на
решенията на участниците, същата, която се ползва на национални и международни 
състезания.

## Авторско право
Файловете в папка solutions и в problem-data не са създадени от мен и
интелектуалната собственост принадлежи на техните автори (участниците и авторите
на задачите съответно). Всичко останало е създадено от мен (Александър Кръстев)
и е предоставено като публично достояние (сиреч, отказвам се от авторските си
права).

[keleved]: http://keleved.com
[isolate]: https://github.com/ioi/isolate
[email]: mailto:aleks.tcr@gmail.com
[github]: https://github.com/Alaxe/noi2-ranking
