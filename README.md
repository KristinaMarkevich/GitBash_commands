# GitBash_commands
Learning how to use GitBash
<hr>

HM1

**1.Посмотреть где я**
```
гдеM@DESKTOP-5LJ56TM MINGW64 ~
$ pwd
/c/Users/M

M@DESKTOP-5LJ56TM MINGW64 ~
$ cd desktop

M@DESKTOP-5LJ56TM MINGW64 ~/desktop
$ pwd
/c/Users/M/desktop
```
**2.Создать папку**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop
$ mkdir newfolder
```
**3.Зайти в папку**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop
$ cd newfolder
```
**4.Создать 3 папки**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ mkdir folder_1 folder_2 folder_3
```
**5.Зайти в любоую папку**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ cd folder_1
```
**6.Создать 5 файлов (3 txt, 2 json)**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder/folder_1
$ touch file_1.txt file_2.txt file_3.txt file_1.json file_2.json
```
**7.Создать 3 папки**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder/folder_1
$ mkdir folder_4 folder_5 folder_6
```
**8.Вывести список содержимого папки**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder/folder_1
$ ls
file_1.json  file_2.json  file_3.txt  folder_5/
file_1.txt   file_2.txt   folder_4/   folder_6/
```
**9.Открыть любой txt файл
10.Написать туда что-нибудь, любой текст
11.Сохранить и выйти**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder/folder_1
$ cat > file_1.txt
O Captain! my Captain! our fearful trip is done,
The ship has weather’d every rack, the prize we sought is won,
The port is near, the bells I hear, the people all exulting,
While follow eyes the steady keel, the vessel grim and daring;
                         But O heart! heart! heart!
                            O the bleeding drops of red,
                               Where on the deck my Captain lies,
                                  Fallen cold and dead.

O Captain! my Captain! rise up and hear the bells;
Rise up—for you the flag is flung—for you the bugle trills,
For you bouquets and ribbon’d wreaths—for you the shores a-crowding,
For you they call, the swaying mass, their eager faces turning;
                         Here Captain! dear father!
                            This arm beneath your head!
                               It is some dream that on the deck,
                                 You’ve fallen cold and dead.

My Captain does not answer, his lips are pale and still,
My father does not feel my arm, he has no pulse nor will,
The ship is anchor’d safe and sound, its voyage closed and done,
From fearful trip the victor ship comes in with object won;
                         Exult O shores, and ring O bells!
                            But I with mournful tread,
                               Walk the deck my Captain lies,
                                  Fallen cold and dead.
```
**12.Выйти из папки на уровень выше**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder/folder_1
$ cd ..
```
**13.Переместить любые 2 файла, которые вы создали, в любую другую папку**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ mv ~/desktop/newfolder/folder_1/{file_2.txt,file_3.txt} ~/desktop/newfolder/folder_2
```
**14.Скопировать любые 2 файла, которые вы создали, в любую другую папку**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ cp folder_1/{file_1.txt,file_1.json} folder_1/folder_4
```
**15.Найти файл по имени**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ find -name "file_1.txt"
./folder_1/file_1.txt
./folder_1/folder_4/file_1.txt
```
 **16.Просмотреть содержимое в реальном времени (команда grep) изучите как она работает**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ grep -i "Captain" folder_1/file_1.txt
O Captain! my Captain! our fearful trip is done,
                               Where on the deck my Captain lies,
O Captain! my Captain! rise up and hear the bells;
                         Here Captain! dear father!
My Captain does not answer, his lips are pale and still,
                               Walk the deck my Captain lies,
```
 **17.Вывести несколько первых строк из текстового файла**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ head -n 3 folder_1/file_1.txt
O Captain! my Captain! our fearful trip is done,
The ship has weather’d every rack, the prize we sought is won,
The port is near, the bells I hear, the people all exulting,
```
 **18.Вывести несколько последних строк из текстового файла**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ tail -n 3 folder_1/file_1.txt
                            But I with mournful tread,
                               Walk the deck my Captain lies,
                                  Fallen cold and dead.
```
 **19.Просмотреть содержимое длинного файла (команда less) изучите как она работает**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ less folder_1/file_1.txt
```
Команда less открывает файл в новом окне, возможен поиск по тексту через функцию /текст - подсвечивает все совпадения.
 
**20.Вывести дату и время**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/newfolder
$ date
Fri Jun  2 13:57:45 RTZ 2023
```

HM2

**1.Сделать папку dir_1**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop
$ mkdir dir_1
```
**2. Зайти в папку dir_1**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop
$ cd dir_1
```
**3.Создать папку inner_dir_1**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ mkdir inner_dir_1
```
**4.Посмотреть где ты находишься**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ pwd
/c/Users/M/desktop/dir_1
```
**5.Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ touch tf_1.txt
```
**6.Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:the first 1, the second 2, the third 3**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ cat > tf_2.txt
the first 1
the second 2
the third 3
```
ctrl + D

**7.Зайти в папку inner_dir_1**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ cd inner_dir_1
```
**8.Через cat сделать текстовый файл tf_3.txt  c любыми строками**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1/inner_dir_1
$ cat > tf_3.txt
Darling, I can show you where my love hides
It's a heart beat
On a hard drive
Yeah, I'm dancing with your soul in my sights
It's a showdown
In the spotlight
```
**9.Через cat добавить в текстовый файл tf_3.txt строку “the second 2”**

**10.Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”**

**11.Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”**

**12.Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”**

**13.Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1/inner_dir_1
$ cat >> tf_3.txt
the second 2
the sec 2
the sec 3
the SeCoNd 2
the seConD 2
```
**14.Сделать текстовый файл tf_4.txt в котором будет 15 строк**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1/inner_dir_1
$ cat > tf_4.txt
If love were mine, if love were mine,
I know what I would do,
I'd take it, spare it,
Give it, share it,
Lend it, spend it, too.
If beauty I could claim for mine,
To hold, to cherish, too,
I'd strive to spread it,
Pour it, shed it,
Till it flowed the whole world through.
But toil—just common toil—is mine;
And so what I shall do
Is strive to take it,
Carve it, make it,
Into love and beauty, too.
```
**15.Сделать текстовый файл tF_5.txt в котором будет 13 строк**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1/inner_dir_1
$ cat > tf_5.txt
One’s beliefs it really seems,
have less weight than do their dreams.
Focus on your dreams each day,
Divvy up your work and play.
Muslims, Christians, Buddhists too
Hold quite different points of view;
all of them cannot be true.
all but we are wrong they say.
Dogma serves to cloud the mind
setting forth a path assigned.
Thinkers dream when they’re inclined.
One s beliefs it really seems,
have less weight than do their dreams.
```
**16. Вывести список всех файлов в папке.**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1/inner_dir_1
$ ls
tf_3.txt  tf_4.txt  tf_5.txt
```
**17. Выйти из папки inner_dir_1**
```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1/inner_dir_1
$ cd ..
```
 **18. Вывести содержимое файла tf_3.txt в терминал**
 ```
$ cat inner_dir_1/tf_3.txt
Darling, I can show you where my love hides
It's a heart beat
On a hard drive
Yeah, I'm dancing with your soul in my sights
It's a showdown
In the spotlight
the second 2
the sec 2
the sec 3
the SeCoNd 2
the seConD 2
```
 **19. Найти путь к файлу tf_4.txt**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ find -name 'tf_4.txt'
./inner_dir_1/tf_4.txt
```
 **20. Отчистить файл tf_4.txt от содержимого без удаления самого файла**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ : > inner_dir_1/tf_4.txt
```
 **21. Найти путь к файлам у которых есть  “tf” в названии**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ find -name '*tf*'
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tf_5.txt
./tf_1.txt
./tf_2.txt
```
**22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ find -iname '*tf*'
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tf_5.txt
./tf_1.txt
./tf_2.txt
```
**23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep "sec" *
grep: inner_dir_1: Is a directory
grep: inner_dir_2: Is a directory
tf_2.txt:the second 2
```
**24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -i "sec" *
grep: inner_dir_1: Is a directory
grep: inner_dir_2: Is a directory
tf_2.txt:the second 2
```
**25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -i -w "sec" *
grep: inner_dir_1: Is a directory
grep: inner_dir_2: Is a directory
```
**26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -i -w "sec" *
grep: inner_dir_1: Is a directory
grep: inner_dir_2: Is a directory
```
**27. Найти строки в файлах где есть комбинация букв “second” в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep "second" *
grep: inner_dir_1: Is a directory
grep: inner_dir_2: Is a directory
tf_2.txt:the second 2
```
**28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -i "second" *
grep: inner_dir_1: Is a directory
grep: inner_dir_2: Is a directory
tf_2.txt:the second 2
```
**29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -r "second"
inner_dir_1/tf_3.txt:the second 2
tf_2.txt:the second 2
```
**30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -l -s "second" *
tf_2.txt
```
**31. Найти все строки во всех файлах где нет комбинации “second”**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ grep -r -v "second"
inner_dir_1/tf_3.txt:Darling, I can show you where my love hides
inner_dir_1/tf_3.txt:It's a heart beat
inner_dir_1/tf_3.txt:On a hard drive
inner_dir_1/tf_3.txt:Yeah, I'm dancing with your soul in my sights
inner_dir_1/tf_3.txt:It's a showdown
inner_dir_1/tf_3.txt:In the spotlight
inner_dir_1/tf_3.txt:the sec 2
inner_dir_1/tf_3.txt:the sec 3
inner_dir_1/tf_3.txt:the SeCoNd 2
inner_dir_1/tf_3.txt:the seConD 2
inner_dir_1/tf_5.txt:One’s beliefs it really seems,
inner_dir_1/tf_5.txt:have less weight than do their dreams.
inner_dir_1/tf_5.txt:Focus on your dreams each day,
inner_dir_1/tf_5.txt:Divvy up your work and play.
inner_dir_1/tf_5.txt:Muslims, Christians, Buddhists too
inner_dir_1/tf_5.txt:Hold quite different points of view;
inner_dir_1/tf_5.txt:all of them cannot be true.
inner_dir_1/tf_5.txt:all but we are wrong they say.
inner_dir_1/tf_5.txt:Dogma serves to cloud the mind
inner_dir_1/tf_5.txt:setting forth a path assigned.
inner_dir_1/tf_5.txt:Thinkers dream when they’re inclined.
inner_dir_1/tf_5.txt:One s beliefs it really seems,
inner_dir_1/tf_5.txt:have less weight than do their dreams.
tf_2.txt:the first 1
tf_2.txt:the third 3
```
**32. Найти только название и путь к файлам где нет комбинации “second”**
 ```
$ grep -r -L "second"
inner_dir_1/tf_4.txt
inner_dir_1/tf_5.txt
tf_1.txt
```
**33. Вывести в терминал 4 последних строк любого текстового файла**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ tail -n 4 inner_dir_1/tf_5.txt
setting forth a path assigned.
Thinkers dream when they’re inclined.
One s beliefs it really seems,
have less weight than do their dreams.
```
**34. Вывести в терминал 4 первые строки любого текстового файла.**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ head -n 4 inner_dir_1/tf_3.txt
Darling, I can show you where my love hides
It's a heart beat
On a hard drive
Yeah, I'm dancing with your soul in my sights
```
**35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ mkdir inner_dir_2 ; cat > inner_dir_2/tf_6.txt
welcome to the heaven!
```
**36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”**
 ```

```
**37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”**
 ```

```
**38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, 
скопировать и вставить эти строки в один новый созданный текстовый файл.**
 ```

```
**39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”**
 ```

```
**40. Просто вывести в терминал строку “Good job!!”**
 ```
M@DESKTOP-5LJ56TM MINGW64 ~/desktop/dir_1
$ echo "Good job!"
Good job!
```
