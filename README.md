# GitBash_commands
**Learning how to use GitBash**

main branch - the first homework

HM2 branch - the second
<hr>


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
