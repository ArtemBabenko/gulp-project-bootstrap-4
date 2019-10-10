## Окружение для разработки веб-проектов на Bootstrap 4 (Болванка)
Готовое окружение для разработки фронтенд составляющей сайтов и интерфейсов админок на Bootstrap 4.

## Требования к окружению
Для создания окружения необходимо иметь следующие установленные инструменты:
-	Node.js
-	Git
-	Gulp
-	Bower (только для версии 1.0.0)

Если у вас данных инструментов нет, то их необходимо установить.

## Установки зависимостей проекта
Для установки зависимостей проекта необходимо в командной строке ввести команды:
-	`npm install`
-	`bower install` (только для версии 1.0.0)

## Как быстро запустить окружение(Подсказки для себя)
1. Устанавливаем зависимости `npm instal` (подгружаем все необходимые файлы). 
2. Сначала запускаем `gulp watch`. Вносим изменения в index.html для появления папки build.(Папка build не успевает создаться и поэтому webserver не запускается)
3. Потом стопим процесс(Ctl+C). Запускаем `gulp watch webserver`. 
(Внимание! В конце присутсвует дефолтная таска. По етому просто при вызове одной команды `gulp` выполняются пункты 2 и 3)
4. Что бы собрать проект для выгрузки в репу `gulp build`. (В файле gulpfile.js подробно коментами расписаны задачи, если очень хочется то можно поковырятся)
5. Весь конечный результат нашей работы(собранный до кучи, минифицированный, пережатый и тд.) находится в папке build, файлы которой мы и размещаем на хостинге.

## От автора(Как использовать окружение ну и подробно писменный гайдик + в видеоформате на youtube)
Обычный режим: в командной строке ввести `gulp`.
Выборочная сборка: в командной строке ввести необходимую задачу. Например, для сборки CSS необходимо ввести команду `css:build`. Список всех доступных задач можно посмотреть в файле gulpfile.js.

Более подробное описание этого окружения доступно на странице: https://itchief.ru/lessons/bootstrap/build-project-with-gulp
