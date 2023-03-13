---
title: Slicer класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells.slicers/slicer/
is_root: false
---
##  Slicer класс
краткое описание Slicer Посмотреть



Тип Slicer предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [title](/cells/ru/python-net/aspose.cells.slicers/slicer/title) | Указывает заголовок текущего объекта Slicer.|
| [alternative_text](/cells/ru/python-net/aspose.cells.slicers/slicer/alternative_text) | Возвращает или задает описательную (альтернативную) текстовую строку объекта Slicer.|
| [is_printable](/cells/ru/python-net/aspose.cells.slicers/slicer/is_printable) | Указывает, доступен ли для печати объект среза.|
| [is_locked](/cells/ru/python-net/aspose.cells.slicers/slicer/is_locked) | Указывает, заблокирована ли форма среза.|
| [placement](/cells/ru/python-net/aspose.cells.slicers/slicer/placement) | Представляет способ прикрепления объекта рисования к ячейкам под ним.<br/> Свойство управляет размещением объекта на рабочем листе.|
| [locked_aspect_ratio](/cells/ru/python-net/aspose.cells.slicers/slicer/locked_aspect_ratio) | Указывает, блокируется ли соотношение сторон.|
| [locked_position](/cells/ru/python-net/aspose.cells.slicers/slicer/locked_position) | Указывает, можно ли перемещать указанный срез или изменять его размер с помощью пользовательского интерфейса.|
| [slicer_cache](/cells/ru/python-net/aspose.cells.slicers/slicer/slicer_cache) |Возвращает объект SlicerCache, связанный со слайсером. Только для чтения.|
| [parent](/cells/ru/python-net/aspose.cells.slicers/slicer/parent) | Возвращает объект Worksheet, представляющий лист, содержащий срез. Только для чтения.|
| [style_type](/cells/ru/python-net/aspose.cells.slicers/slicer/style_type) | Укажите тип стиля встроенного слайсера<br/> тип по умолчанию — SlicerStyleLight1|
| [name](/cells/ru/python-net/aspose.cells.slicers/slicer/name) | Возвращает или задает имя указанного слайсера|
| [caption](/cells/ru/python-net/aspose.cells.slicers/slicer/caption) | Возвращает или задает заголовок указанного слайсера.|
| [caption_visible](/cells/ru/python-net/aspose.cells.slicers/slicer/caption_visible) | Возвращает или задает, отображается ли заголовок, отображающий Caption слайсера.<br/> Значение по умолчанию верно|
| [number_of_columns](/cells/ru/python-net/aspose.cells.slicers/slicer/number_of_columns) | Возвращает или задает количество столбцов в указанном слайсере.|
| [left_pixel](/cells/ru/python-net/aspose.cells.slicers/slicer/left_pixel) | Возвращает или задает смещение формы среза по горизонтали относительно левого столбца в пикселях.|
| [top_pixel](/cells/ru/python-net/aspose.cells.slicers/slicer/top_pixel) | Возвращает или задает вертикальное смещение формы среза от ее верхней строки в пикселях.|
| [width](/cells/ru/python-net/aspose.cells.slicers/slicer/width) | Возвращает или задает ширину указанного среза в пунктах.|
| [width_pixel](/cells/ru/python-net/aspose.cells.slicers/slicer/width_pixel) | Возвращает или задает ширину указанного среза в пикселях.|
| [height](/cells/ru/python-net/aspose.cells.slicers/slicer/height) | Возвращает или задает высоту указанного среза в пунктах.|
| [height_pixel](/cells/ru/python-net/aspose.cells.slicers/slicer/height_pixel) |Возвращает или задает высоту указанного среза в пикселях.|
| [column_width_pixel](/cells/ru/python-net/aspose.cells.slicers/slicer/column_width_pixel) | Получает или задает ширину в пикселях для каждого столбца среза.|
| [column_width](/cells/ru/python-net/aspose.cells.slicers/slicer/column_width) | Возвращает или задает ширину (в пунктах) каждого столбца в слайсере.|
| [row_height_pixel](/cells/ru/python-net/aspose.cells.slicers/slicer/row_height_pixel) | Возвращает или задает высоту в пикселях каждой строки в указанном срезе.|
| [row_height](/cells/ru/python-net/aspose.cells.slicers/slicer/row_height) | Возвращает или задает высоту в пунктах каждой строки в указанном срезе.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add_pivot_connection(pivot)](/cells/ru/python-net/aspose.cells.slicers/slicer/add_pivot_connection/#aspose.cells.pivot.PivotTable) | Добавляет соединение со сводной таблицей.|
| [remove_pivot_connection(pivot)](/cells/ru/python-net/aspose.cells.slicers/slicer/remove_pivot_connection/#aspose.cells.pivot.PivotTable) | Удаляет подключение к сводной таблице.|
| [refresh()](/cells/ru/python-net/aspose.cells.slicers/slicer/refresh/#) | Обновление слайсера. Между тем, обновление и расчет относительных сводных таблиц.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.cells.slicers import SlicerStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
slicerIndex = slicers.add(pivot, "E12", "fruit")
slicer = slicers[slicerIndex]
slicer.style_type = SlicerStyleType.SLICER_STYLE_LIGHT2
items = slicer.slicer_cache.slicer_cache_items
item = items[0]
item.selected = False
# do your business
book.save("out.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.slicers](..)
