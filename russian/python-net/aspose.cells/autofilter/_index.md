---
title: AutoFilter класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter класс
Представляет автофильтрацию для указанного рабочего листа.



Тип AutoFilter предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [sorter](/cells/ru/python-net/aspose.cells/autofilter/sorter) | Получает сортировщик данных.|
| [range](/cells/ru/python-net/aspose.cells/autofilter/range) | Представляет диапазон, к которому применяется указанный автофильтр.|
| [show_filter_button](/cells/ru/python-net/aspose.cells/autofilter/show_filter_button) | Указывает, видна ли кнопка автофильтра для этого столбца.|
| [filter_columns](/cells/ru/python-net/aspose.cells/autofilter/filter_columns) | Получает коллекцию столбцов фильтра.|


###  Методы
| Метод| Описание|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/ru/python-net/aspose.cells/autofilter/remove_filter/#int-str) |Удаляет фильтр для столбца фильтра.|
| [remove_filter(field_index)](/cells/ru/python-net/aspose.cells/autofilter/remove_filter/#int) | Удалите определенный фильтр.|
| [custom(field_index, operator_type1, criteria1)](/cells/ru/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Фильтрует список с пользовательскими критериями.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/ru/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Фильтрует список с пользовательскими критериями.|
| [refresh()](/cells/ru/python-net/aspose.cells/autofilter/refresh/#) | Обновите автоматические фильтры, чтобы скрыть или отобразить строки.|
| [refresh(hide_rows)](/cells/ru/python-net/aspose.cells/autofilter/refresh/#bool) | Получает индексы всех скрытых строк.|
| [set_range(row, start_column, end_column)](/cells/ru/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Задает диапазон, к которому применяется указанный автофильтр.|
| [get_cell_area()](/cells/ru/python-net/aspose.cells/autofilter/get_cell_area/#) | Получает [CellArea](/cells/ru/python-net/aspose.cells/cellarea), к которому применяется указанный автофильтр.|
| [add_filter(field_index, criteria)](/cells/ru/python-net/aspose.cells/autofilter/add_filter/#int-str) | Добавляет фильтр для столбца фильтра.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/ru/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Добавляет фильтр даты.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/ru/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Удаляет фильтр даты.|
| [filter(field_index, criteria)](/cells/ru/python-net/aspose.cells/autofilter/filter/#int-str) | Фильтрует список по заданным критериям.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/ru/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Отфильтровать первые 10 элементов в списке|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/ru/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Добавляет динамический фильтр.|
| [add_font_color_filter(field_index, color)](/cells/ru/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Добавляет фильтр цвета шрифта.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/ru/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Добавляет фильтр цвета заливки.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/ru/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Добавляет фильтр значков.|
| [match_blanks(field_index)](/cells/ru/python-net/aspose.cells/autofilter/match_blanks/#int) | Совпадение со всеми пустыми ячейками в списке.|
| [match_non_blanks(field_index)](/cells/ru/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Совпадение со всеми непустыми ячейками в списке.|
| [show_all()](/cells/ru/python-net/aspose.cells/autofilter/show_all/#) | Показать все строки.|



###  Пример

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [CellArea](/cells/ru/python-net/aspose.cells/cellarea)
