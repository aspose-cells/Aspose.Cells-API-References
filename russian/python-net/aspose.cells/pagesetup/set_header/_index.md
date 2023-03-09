---
title: set_header метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 200
url: /ru/python-net/aspose.cells/pagesetup/set_header/
is_root: false
---
##  set_header(section, header_script) {#int-str}
Задает сценарий, форматирующий заголовок файла Excel.



```python
def set_header(self, section, header_script):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| section | int | 0: левая часть, 1: центральная часть, 2: правая часть.|
| header_script | str | Скрипт формата заголовка.|
###  Примечания

Команды скрипта:

| Команда| Описание|
| :- | :- |
| &П| Текущий номер страницы|
| &N| Количество страниц|
| &D| Текущая дата|
| &Т| Текущее время|
| &А| Имя листа|
| &F| Имя файла без пути|
| &"<FontName>"| Название шрифта, например: &"Arial"|
| &"<FontName>, <FontStyle>"| Название и стиль шрифта, например: &"Arial,Bold"|
| &<FontSize>| Размер шрифта.Если за этой командой следует простое число, которое будет напечатано в заголовке, оно будет отделено от высоты шрифта символом пробела.|
| &К<RRGGBB>|Цвет шрифта, например (КРАСНЫЙ): &KFF0000|
| &Г| Сценарий изображения|

Например: "&Arial,Bold&8Примечание к заголовку"


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PageSetup](/cells/ru/python-net/aspose.cells/pagesetup)
