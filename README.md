# Лабораторная работа №6

## 1. Цель работы

Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

## 2. Основная часть работы

### Форк репозитория

Создается копия репозитория в личное хранилище, копируются обе ветки: master и branch1

![Форк репозитория](screenshot/добавление_файла.png)

### Настройка клиента git

Задается имя пользователя согласно требованиям, указанным в ЛР. Почта уже была задана ранее. 

![Настройки GitBash](screenshot/настройки.png)

### Клонирование репозитория на компьютер

Создается папка, в которую будет клонирован репозиторий. 

![Клонирование репозитория](screenshot/клонирование.png)

### Добавление файла через интерфейс GitHub

В личном репозитории необходимо воспользоваться кнопкой ```add file``` >> ```create new file```. В основкую ветку был добавлен текстовый файл ```file.txt```.

![Добавление файла](screenshot/добавление_файла.png)

### Подтягивание изменений в локальный репозиторий

Подтягиваем добавление нового файла в репозиторий на компьютере.

![Подтягивание изменений](screenshot/подтягивание_изменений.png)

### История операций для каждой ветки

Для начала просматривается история для основной ветки, затем происхолдит переключение на branch1 и просмотр ее истории.

![История операций](screenshot/история_операций.png)

### Просмотр последних изменений

Просмотр последнего коммита выполняется для веток в обратном порядке аналогично предыдущему шагу - сначала для branch1, затем для master.

![Последние изменения](screenshot/последние_изменения.png)

### Слиние в одну ветку

Изначальная попытка слить ветки не увенчивается успехом, возник конфликт веток. В индекс не былы добавлены изменения файла mergefile.txt. Необходимо добавить изменения в основную ветку, после чего повторно применить команду слияния.

![Слияние в одну ветку](screenshot/слияние.png)

### Удаление побочной ветки

После слияния двух веток, ветка branch1 удаляется.

![Удаление ветки branch1](screenshot/удаление.png)

### Изменения в файле

Файл ```file.txt``` был изменен несколько раз, изменения были зафиксировны коммитами.

![Изменения текстового файла](screenshot/изменения_файла.png)

### Откат коммита

Для отката необходимо указать хеш того коммита, на который произойдет откат. Все изменения, сделанные после этого коммита будут отменены.

![Откат коммита](screenshot/откат.png)

### Создание ветки для отчета

Для отчета и демонстрации проделанной работы создается новая ветка ```report_branch```.

![Новая ветка](screenshot/новая_ветка.png)

## 3. Логи команд

В процессе выполнения лабораторной работы были использованы следующие команды:

```
git config --global user.name "4318 Loknovskaya A.D."
git cofig user.name
git config user.email
git clone https://github.com/AnnLoknovskaya/LR6
git pull origin master
git log --oneline
git checkout branch1
git checkout master
git show
git merge branch1
git status
git add ...
git commit -m "comment"
git push origin --delete branch1
git reset --hard 438ee03
git checkout -b report_branch
git push origin ...
```

## 4. История операций в форматированном виде
![История операций](screenshot/форматир.png)

## 5. Выводы

В ходе выполнения лабораторной работы были изучены базовые возможности системы управления версиями, получен опыт работы с Git Api, получен опыт работы с локальным и удаленным репозиторием.












































