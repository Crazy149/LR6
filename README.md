# LR6
Лабораторная работа №6

Цель лабораторной работы: изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

**Выполнение работы**

* Клонировать совй личный удаленный репозиторий на компьютер.
![Клонировать свой личный удаленный репозиторий](screen/1.jpg)
``` bash
 git clone https://github.com/Crazy149/LR6.git
```

* Добавить файл через интерфейс GitHub. Подянуть изменения в локальный репозиторий
![Добавить файл через интерфейс GitHub. Подянуть изменения в локальный репозиторий](screen/2.jpg)
```bash
git pull
```

* Получить историю операций для каждой из веток
![Получить историю операций для каждой из веток](screen/3.jpg)
```bash
git log --graph
```

* Посмотреть последние изменения.
![Получить историю операций для каждой из веток](screen/4.jpg)
```bash
git log
```
* Выполнить слияние в ветку master, разрешив конфликт.
![Выполнить слияние в ветку master, разрешив конфликт](screen/5.jpg)
![Выполнить слияние в ветку master, разрешив конфликт](screen/6.jpg)
```bash
git branch newbranch
git checkout newbranch
git add . 
git commit 
git checkout master
git merge 
```

* Удалить побочную ветку после успешного слияния.
![Удалить побочную ветку после успешного слияния](screen/7.jpg)
```bash
git branch -d newbranch
```

* Сделать изменения и зафиксировать их, оставляя коментарии.
![Сделать изменения и зафиксировать их, оставляя коментарии](screen/8.jpg)
```bash
git add . 
git commit
```
* Сделать откат коммита
![Сделать откат коммита](screen/9.jpg)

* Получена история операций в форматированном виде
![Получена история операций в форматированном виде](screen/10.jpg)

* Отправить локальные изменения в сетевое хранилище GitHub
```bash
git push -u origin 
```