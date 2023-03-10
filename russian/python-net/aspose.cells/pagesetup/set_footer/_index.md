---
title: set_footer метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 180
url: /ru/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
Задает сценарий, форматирующий нижний колонтитул файла Excel.



```python
def set_footer(self, section, footer_script):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| section | int | 0: левая часть, 1: центральная часть, 2: правая часть.|
| footer_script | str | Скрипт формата нижнего колонтитула.|
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
| &<FontSize>| Размер шрифта. Если за этой командой следует простое число, которое будет напечатано в заголовке, оно будет отделено от высоты шрифта символом пробела.|
| &К<RRGGBB>|Цвет шрифта, например (КРАСНЫЙ): &KFF0000|
| &Г| Сценарий изображения|

Например: "&Arial,Bold&8Footer Note"


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PageSetup](/cells/ru/python-net/aspose.cells/pagesetup)
