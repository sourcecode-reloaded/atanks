README для программы Atomic Tanks 
============================================

Что такое Atomic Tanks?
========================

Atomic Tanks - это игра, в которой вы управляете мощным танком.
Ваша задача - уничтожить танки противника и не пропасть самому.
Игроки могут покупать различное оружие и снаряжение. Сражения
происходят в пошаговом режиме. Побеждает единственный
уцелевший танк.


Как мне получить/установить Atomic Tanks?
===================================

Чтобы получить Atomic Tanks, зайдите на наш сайт:
http://atanks.sourceforge.net
Затем зайдите в секцию "Download" и скачайте самую
последнюю версию Atomic Tanks.

Внимание: Если у вас уже есть скомпилированная (запускаемая)
копия Atomic Tanks, вам понадобится графический пакет Allegro.
Подробнее на сайте: http://allegro.cc/
Помимо этого, если вы собираетесь скомпилировать Atomic
Tanks из исходников, вам потребуется development-пакет
Allegro.
Все эти пакеты могут быть найдены на странице:
http://allegro.cc/files
Пользователи Linux могут скачать вышеназванные пакеты
с помощью менеджера пакетов в своём дистрибутиве.
В Fedora Linux эти пакеты называются "allegro"
и "allegro-devel". В Ubuntu эти пакеты называются
"liballegro*" и "liballegro*-dev", где "*" - номер
последней версии.


Если вы используете уже собранную (запускаемую) копию
Atomic Tanks, загляните в следующий раздел, описывающий
запуск игры. Дальнейший текст этого раздела посвящён
компиляции игры из исходников.


Прежде чем компилировать Atomic Tanks, проверьте,
установлены ли библиотеки Allegro (см. выше).
После этого откройте командную консоль (shell, bash, etc)
и перейдите в директорию, в которой находится архив
с исходниками Atomic Tanks.
Архив версии 6.0 называется "atanks-6.0.tar.gz".

После этого выполните следующие команды:

tar zxf atanks-6.0.tar.gz
cd atanks-6.0



Дальнейшие настройки зависят от ваших предпочтений.

Команда
make
устанавливает игру в папку с распакованным архивом.
Все настройки сохраняются в этой папке.
Можно сразу же запускать команду "./atanks", чтобы
начать играть. ;)


Команды
make system
make install
устанавливают Atomic Tanks в директории по умолчанию.
Бинарные файлы будут перемещены в /usr/games/bin
Данные игры будут перемещены в /usr/share/games/atanks


Команда
make winuser
устанавливает Atomic Tanks в ту же папку, в которой
находятся исходники, для пользователя ОС Windows.


Команда
make osxuser
устанавливает Atomic Tanks в ту же папку, в которой
находятся исходники, для пользователя Mac OS X.



После выполнения соответствующих команд можно
запускать игру.
Если у вас возникают сообщения об ошибках во время
выполнения make, пожалуйста, изучите последний раздел
этого документа, посвящённый сообщениям об ошибках.






Как запустить игру?
====================================

Вы можете запустить игру, введя "./atanks" в
командной консоли или дважды щёлкнув по
запускаемому файлу в файловом менеджере.
При запуске Atomic Tanks использует специально подобранные
настройки по умолчанию, так что в большинстве случаев
использовать опции командной строки нет необходимости.
Тем не менее, игра поддерживает следующие команды:

./atanks -h   (Выводит список разработчиков, опции командной строки и завершает работу.)
./atanks -fs  (Запускает игру в полноэкранном режиме.)
./atanks --windowed  (Запускает игру в оконном режиме. Это режим по умолчанию.)
./atanks --nosound  (Запускает игру без звука.)
./atanks --noname   (Отключает отображение имён игроков над танками.)
./atanks --width <number>  (Запускает игру с указанной в пикселях шириной экрана.)
./atanks --tall <number>  (Запускает игру с указанной в пикселях высотой экрана.)
./atanks --datadir <data directory>  (Указывает директорию с данными для Atomic Tanks.)
./atanks --depth <number>  (Устанавливает глубину цвета. Допустимые значения: 16, 32)
./atanks --noconfig   (Сбрасывает конфигурацию, использует настройки по умолчанию.)
./atanks --nonetwork  (Не даёт Atanks подключаться к сети.)
./atanks --nobackground  (Убирает зелёный фон в главном меню. Помогает от глюков на 64-битных системах.)

Большинство этих опций могут использоваться вместе, за исключением "-fs"
для включения полноэкранного режима.
Простая команда "./atanks" запускает игру с теми же параметрами, что и команда:
./atanks --windowed --width 800 --tall 600 --datadir . depth 32




Как мне создать игрока для себя?
================================================

Сразу после запуска Atomic Tanks вам понадобится создать себе
игрока. Для этого щёлкните по кнопке "Игроки" ("Players")
и выберите пункт "Создать нового" ("Create new").
Введите желаемое имя для игрока (не забудьте нажать Enter)
и выберите цвет для себя. Это все основные настройки;
можно щёлкнуть кнопку "Okay".
После этого щёлкните по кнопке "Назад" ("Back") и затем по
желанной кнопке "Играть" ("Play")!

Сразу после этого откроется меню новой игры, в которой вам
будет предложено выбрать те танки, которые будут участвовать
в сражениях. Не забудьте выбрать себя (рядом с вами есть
фиолетовый кружок) и несколько танков противника!
Если вы начинающий игрок, лучше выбирать себе противников
меньшего уровня (чем меньше зелёных полос рядом с именем танка,
тем проще будет его победить).
После этого выберите количество раундов, имя игры (необязательно)
и нажмите "Okay"!

На следующем экране вам будет предложено купить себе оружие
и снаряжение на следующий раунд. Этот экран будет появляться перед
каждым новым раундом, так что у вас будет время хорошенько
попрактиковаться и подобрать себе хорошую комбинацию оружия.
Щёлкнув левой кнопкой мыши, вы покупаете оружие. Правая кнопка
мыши продаёт оружие или отменяет покупку.
После того, как вы закупились, нажмите "Готово".

После этого начинается игра.
Ваша задача: используя всё то вооружение, которое вы приобрели,
уничтожить все танки противника и при этом уцелеть самому.
Используйте стрелки влево и вправо для изменения угла выстрела,
стрелки вверх и вниз для изменения силы (дальности) выстрела
и стреляйте кнопкой "Пробел"!
Если вы купили какое-нибудь оружие, используйте клавиши
"Z" и "C" для выбора нужного типа снаряда или ракеты.

В каждом раунде побеждает единственный уцелевший танк.

За каждое попадание в противника вплоть до его уничтожения
вы получаете дополнительные деньги, которые вы можете потратить
после каждого раунда.



Где можно сообщить об ошибке или посоветовать что-либо разработчикам?
=========================================

Atomic Tanks - здоровская игра! ;)
Но она не совершенна и находится в постоянной разработке.
Мы, разработчики, всегда стремимся улучшить игру.
Если у вас возникли проблемы с установкой или запуском
Atomic Tanks, пожалуйста, сообщите нам на форуме:
http://atanks.forumwise.com/
Мы благодарны каждому, кто сообщил об ошибке.
Пожалуйста, сообщите как можно больше деталей (версия
операционной системы, версия игры, особенности вашего
компьютера, которые могли повлиять на работу игры) -
это облегчит нам задачу и позволит исправить ошибку
и помочь вам в кратчайшие сроки.

Авторы перевода:
MyO <myothehedgefox@gmail.com>
Sergi <grayman2000@gmail.com>

