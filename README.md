# Infinity Paradise (Изменённый код Paradise)
[![Build Status](https://travis-ci.org/infinitystation/ParadiseSS13.svg?branch=master)](https://travis-ci.org/infinitystation/ParadiseSS13)

[Веб-сайт сообщества Paradise](http://www.nanotrasen.se/) - [Оригинальный код Paradise](https://github.com/ParadiseSS13/Paradise) - [IRC разработчиков Paradise](http://www.nanotrasen.se/phpBB3/viewtopic.php?f=10&t=1113)
[Веб-сайт Infinity](https://infinity.so/)

---

### ЗАГРУЗКА
Есть два способа получить код. Варианты будут описаны ниже:

1. Вы можете скачать напрямую из этого репозитория .zip файл, достаточно просто нажать [суда](https://github.com/infinitystation/ParadiseSS13/archive/master.zip)

2. Этот вариант подходит если Вы собираетесь работать с нашим репозиторием, для этого Вам нужен любой Git клиент.
Откройте командную строку Git клиента и скопируйте в неё следующее:

    git clone https://github.com/infinitystation/ParadiseSS13.git

Это займёт больше времени на загрузку, но при данном методе вам будет легче принимать изменения, не перекачивая репозиторий.

### УСТАНОВКА

Для установки Вам потребуется программа для установки и запуска.
Взять её Вы можете [тут](http://www.byond.com/).

Следующим шагом будет компилирование скачанных файлов.  
Откройте paradise.dme двойным кликом, нажмите в верхней панели раздел Build и нажмите на кнопку компилирования или нажмите комбинацию клавиш Ctrl+K.  
Потребуется немного времени на данный процесс, после окончания Вам должно высветиться данное сообщение:

    saving paradise.dmb (DEBUG mode)

    paradise.dmb - 0 errors, 0 warnings

Если будут какие либо проблемы с компилированиям то возможно часть файлов была потеряна при загрузке.
Если проблема была так и не устранена, обратитесь на наш форум за помощью.

---

### КОНФИГУРАЦИЯ

Файл config.txt был настроен для игры на нашем сервере, но Вы можете настроить его по своему желанию для локального сервера.

Если Вы желаете получить на локальном сервере права администратора, найдите в папке config текстовый файл admins.txt
Введите в данном файле представленную ниже информацию, заменяя слова "byondkey" на Ваш логин клиента и "rank" на "Admin"

	byondkey - Rank

Важно: писать свой byond-логин надо заменяя заглавные буквы на строчные, вместо пробелов писать слитно.

---

### ОБНОВЛЕНИЕ

Перед обновлением, рекомендуем Вам сохранить вашу конфигурацию в папке /config если вы вносили туда изменения.

Если вы используете метод распаковки .zip файла:
Вам нужно скачать .zip файл и распаковать в пустую папку обновлённый билд, после чего перенести ваши конфиги в новый билд.

Если вы используете git метод, введите в консоль клиента следующую команду:

    git pull

Когда обновление закончится, перекопируйте сохранённые конфиги обратно, если нужно.

После обновления перекомпилируйте билд.

---

### SQL Setup

The SQL backend for the library and stats tracking requires a MySQL server.  
Your server details go in /config/dbconfig.txt,
and the SQL schema is in /SQL/paradise_schema.sql or /SQL/paradise_schema_prefix.sql,
depending on if you want table prefixes.  
More detailed setup instructions are located on /tg/station's wiki: http://www.tgstation13.org/wiki/Downloading_the_source_code#Setting_up_the_database

---

### IRC Bot Setup

Included in the repo is an IRC bot capable of relaying adminhelps to a specified IRC
channel/server (thanks to Skibiliano).  
Instructions for bot setup are included in the /bot/ folder,
along with the bot/relay script itself.

### LICENSE

Paradise is licensed under the GNU Affero General Public License version 3.
As of 5th January 2015 any new contributions are licensed under the AGPL as well,
if you wish to submit code under the GPL v3 then commits and files must be marked as such
in comments. If you wish to use our code in a closed source manner you may use anything
before commit 445615b8439bf606ff204a42c8e7b6b69d983255,
which is licensed under GPL v3.
The major change here is that if you host a server using any code licensed under AGPL you
are required to provide full source code for your servers users as well,
including addons and modifications you have made.

See [this](https://www.gnu.org/licenses/why-affero-gpl.html) for more information.

Any files located in the
`Paradise/goon`,
`Paradise/icons/goonstation`, or
`Paradise/sound/goonstation`
directories, or any subdirectories of mentioned directories are licensed under the
Creative Commons 3.0 BY-NC-SA license
(https://creativecommons.org/licenses/by-nc-sa/3.0)

All other assets including icons and sound files are licensed under the
Creative Commons 3.0 BY-SA license (https://creativecommons.org/licenses/by-sa/3.0/),
unless otherwise indicated.



