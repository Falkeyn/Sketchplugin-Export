### Экспорт артбордов для публикации на UI

Берет все артборды (artboard) из sketch-файла и сохраняет в папку с исходником в формате PNG. Для каждой страницы (page) создается отдельная папка и ее артборды складываются туда.

В названии файлов меняет пробелы на «_», заменяет «й» на «и» (решает проблему с svn).

Команды плагина:<br />
<img src="https://github.com/Falkeyn/Screenshots/blob/master/Sketchplugin-Export/menu.png?raw=true">

- **All Pages** — экспортирует разом все артборды со всех страниц
- **Current Page** — экспортирует артборды только текущей страницы
- **Selected Artboards** — экспортирует только выбранные артборды

*При использовании **Current Page** если выбран хотя бы один артборд, то плагин экспортирует только выбранное. При экспорте выбранного не обновляется индексный файл.*

##### Опции

- Любой артборд или страницу можно исключить из экспорта поставив в начало названия «-» (минус)
- Если у страницы поставить в начало названия «*» (звездочка) то артборды этой страницы не будут группироваться в папку, а экспортируются рядом с исходником

В названии файлов меняет пробелы на «_» и подставляет в начало порядковый номер артборда (в том порядке как они идут на левой панели). Т.е. поддерживает нужный порядок, и артбордам можно давать нормальные понятные имена.

##### Пример

В исходнике:<br />
<img src="https://github.com/Falkeyn/Screenshots/blob/master/Sketchplugin-Export/layers-list.png?raw=true">

Результат экспорта:<br />
<img src="https://github.com/Falkeyn/Screenshots/blob/master/Sketchplugin-Export/file-list.png?raw=true">

Индексный файл:<br />
<img src="https://github.com/Falkeyn/Screenshots/blob/master/Sketchplugin-Export/index.png?raw=true">
