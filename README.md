## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Выполнить инструкцию учебного материала
- [x] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial
/* Создание переменных*/
```bash
$ export GITHUB_USERNAME=<имя_пользователя>
$ export GIST_TOKEN=<сохраненный_токен>
/*Текстовый редактор (выбрано vim)*/
$ alias edit=<nano|vi|vim|subl>
```
/* Установка gitsup*/
```bash
$ npm install -g gistup
```
/* Сохранение токена в файл*/
```bash
$ cat > ~/.gistup.json <<EOF
{
  "token": "${GIST_TOKEN}"
}
EOF
```
/* Создание новых директорий*/
```bash
$ cd ~
$ mkdir -p workspace/labs/projects/
$ mkdir -p workspace/labs/tasks/
$ mkdir -p workspace/labs/reports/
```

## Report
```bash
/*Переход в "/workspace/labs/"*/
$ cd ~/workspace/labs/
/*Создание переменной*/
$ export LAB_NUMBER=02
/*Клонирование*/
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
/*Создание новой директории*/
$ mkdir reports/lab${LAB_NUMBER}
/*Копирования файлов*/
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
/*Переход в "reports/lab02"*/
$ cd reports/lab${LAB_NUMBER}
/*Редактирование файла*/
$ edit REPORT.md
$ gistup -m "lab${LAB_NUMBER}"
```

## Links

### Unix commands

- [ar](https://en.wikipedia.org/wiki/Ar_(Unix)) - архивирует файлы и директории
- [cat](https://en.wikipedia.org/wiki/Cat_(Unix)) - последовательно выводит файлы, объединяя их в отдельный поток
- [cd](https://en.wikipedia.org/wiki/Cd_(command)) - смена директории 
- [cp](https://en.wikipedia.org/wiki/Cp_(Unix)) - копирование файлов или директорий
- [cut](https://en.wikipedia.org/wiki/Cut_(Unix)) - вырезка данных из файла
- [echo](https://en.wikipedia.org/wiki/Echo_(command)) - отображает строку текста
- [env](https://en.wikipedia.org/wiki/Env_(shell)) - исполняет команду с изменением окружения
- [ex](https://en.wikipedia.org/wiki/Ex_(editor)) - расширенный тестовый редактор с возможностью экранного редактирования 
- [file](https://en.wikipedia.org/wiki/File_(command)) - определяет тип файла
- [find](https://en.wikipedia.org/wiki/Find) - поиск файлов
- [ls](https://en.wikipedia.org/wiki/Ls) - печатает в стандартный вывод содержимое каталогов
- [man](https://en.wikipedia.org/wiki/Man_page) - форматирует и выводит справочные страницы
- [mkdir](https://en.wikipedia.org/wiki/Mkdir) - создает директорию
- [mv](https://en.wikipedia.org/wiki/Mv) - перемещает файлы или директории
- [nm](https://en.wikipedia.org/wiki/Nm_(Unix)) - печатает информацию о бинарных файлах
- [ps](https://en.wikipedia.org/wiki/Ps_(Unix)) - отчет о рабочих процессах
- [pwd](https://en.wikipedia.org/wiki/Pwd) - текущий рабочий каталог
- [rm](https://en.wikipedia.org/wiki/Rm_(Unix)) - удаляет файлы или директории
- [sed](https://en.wikipedia.org/wiki/Sed) - потоковый текстовый редактор
- [touch](https://en.wikipedia.org/wiki/Touch_(Unix)) - устанавливает время последнего доступа в файл)

### Package Managers

- [apt](http://help.ubuntu.ru/wiki/apt) | [dnf](https://en.wikipedia.org/wiki/DNF_(software)) | [yum](https://fedoraproject.org/wiki/Yum/ru)
- [brew](https://brew.sh) | [linuxbrew](http://linuxbrew.sh)
- [npm](https://docs.npmjs.com)

### Software

- [curl](https://www.gitbook.com/book/bagder/everything-curl/details)
- [wget](https://www.gnu.org/software/wget/manual/wget.pdf)
- [clang](https://clang.llvm.org)
- [g++](https://gcc.gnu.org/onlinedocs/gcc-4.0.2/gcc/G_002b_002b-and-GCC.html)
- [make](https://en.wikipedia.org/wiki/Make_(software))
- [open](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/open.1.html)
- [openssl](https://www.openssl.org)
- [nano](https://www.nano-editor.org)
- [tree](https://linux.die.net/man/1/tree)
- [vim](http://www.vim.org)

```
Copyright (c) 2017 Братья Вершинины
```
