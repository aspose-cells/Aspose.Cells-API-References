---
title: PivotField класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells.pivot/pivotfield/
is_root: false
---
##  PivotField класс
Представляет поле в отчете сводной таблицы.



Тип PivotField предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [pivot_items](/cells/ru/python-net/aspose.cells.pivot/pivotfield/pivot_items) | Получает элементы сводки поля сводки|
| [range](/cells/ru/python-net/aspose.cells.pivot/pivotfield/range) | Получает диапазон группы сводного поля|
| [is_calculated_field](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_calculated_field) | Указывает, является ли указанное поле сводной таблицы вычисляемым полем.|
| [base_index](/cells/ru/python-net/aspose.cells.pivot/pivotfield/base_index) | Представляет индекс PivotField в базовых полях PivotField.|
| [position](/cells/ru/python-net/aspose.cells.pivot/pivotfield/position) | Представляет индекс PivotField в PivotFields.|
| [name](/cells/ru/python-net/aspose.cells.pivot/pivotfield/name) | Представляет имя PivotField.|
| [display_name](/cells/ru/python-net/aspose.cells.pivot/pivotfield/display_name) | Представляет отображаемое имя PivotField.|
| [is_auto_subtotals](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_auto_subtotals) | Указывает, отображаются ли в указанном поле автоматические промежуточные итоги.Значение по умолчанию — true.|
| [drag_to_column](/cells/ru/python-net/aspose.cells.pivot/pivotfield/drag_to_column) | Указывает, можно ли перетащить указанное поле в положение столбца.<br/> Значение по умолчанию верно.|
| [drag_to_hide](/cells/ru/python-net/aspose.cells.pivot/pivotfield/drag_to_hide) | Указывает, можно ли перетащить указанное поле в скрытое положение.<br/> Значение по умолчанию верно.|
| [drag_to_row](/cells/ru/python-net/aspose.cells.pivot/pivotfield/drag_to_row) | Указывает, можно ли перетащить указанное поле в позицию строки.<br/> Значение по умолчанию верно.|
| [drag_to_page](/cells/ru/python-net/aspose.cells.pivot/pivotfield/drag_to_page) | Указывает, можно ли перетаскивать указанное поле на позицию страницы.<br/> Значение по умолчанию верно.|
| [drag_to_data](/cells/ru/python-net/aspose.cells.pivot/pivotfield/drag_to_data) |Указывает, можно ли перетащить указанное поле в позицию данных.<br/> Значение по умолчанию верно.|
| [is_multiple_item_selection_allowed](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_multiple_item_selection_allowed) | указывает, может ли поле иметь несколько элементов<br/>выбрано в поле страницы<br/> Значение по умолчанию неверно.|
| [is_repeat_item_labels](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_repeat_item_labels) | указывает, может ли поле повторять метки элементов<br/> Значение по умолчанию неверно.|
| [is_include_new_items_in_filter](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_include_new_items_in_filter) | указывает, может ли поле включать новые элементы в ручном фильтре<br/> Значение по умолчанию неверно.|
| [is_insert_page_breaks_between_items](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_insert_page_breaks_between_items) | указывает, может ли поле вставлять разрывы страниц между элементами<br/>вставлять разрыв страницы после каждого элемента<br/> Значение по умолчанию неверно.|
| [show_all_items](/cells/ru/python-net/aspose.cells.pivot/pivotfield/show_all_items) | Указывает, отображаются ли все элементы в отчете сводной таблицы,<br/>даже если они не содержат сводных данных.<br/>показать элементы без данных<br/> Значение по умолчанию неверно.|
| [non_auto_sort_default](/cells/ru/python-net/aspose.cells.pivot/pivotfield/non_auto_sort_default) | Указывает, является ли операция сортировки, которая будет применена к этому сводному полю, операцией автосортировки или простой сортировкой данных.|
| [is_auto_sort](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_auto_sort) | Указывает, сортируется ли указанное поле сводной таблицы автоматически.|
| [is_ascend_sort](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_ascend_sort) | Указывает, сортируется ли указанное поле сводной таблицы автоматически по возрастанию.|
| [auto_sort_field](/cells/ru/python-net/aspose.cells.pivot/pivotfield/auto_sort_field) | Представляет индекс поля автоматической сортировки.<br/> -1 означает сам PivotField, другие означают положение полей данных.|
| [is_auto_show](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_auto_show) | Указывает, отображается ли указанное поле сводной таблицы автоматически, только для Excel 2003.|
| [is_ascend_show](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_ascend_show) | Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию.|
| [auto_show_count](/cells/ru/python-net/aspose.cells.pivot/pivotfield/auto_show_count) |Представлять количество верхних или нижних элементов<br/> которые автоматически отображаются в указанном поле сводной таблицы.|
| [auto_show_field](/cells/ru/python-net/aspose.cells.pivot/pivotfield/auto_show_field) | Представляет индекс поля автоматического отображения. -1 означает сам PivotField.<br/> Это должен быть индекс полей данных.|
| [function](/cells/ru/python-net/aspose.cells.pivot/pivotfield/function) | Представляет функцию, используемую для суммирования поля данных сводной таблицы.|
| [data_display_format](/cells/ru/python-net/aspose.cells.pivot/pivotfield/data_display_format) | Представляет, как отображать значения, содержащиеся в поле данных.|
| [base_field_index](/cells/ru/python-net/aspose.cells.pivot/pivotfield/base_field_index) | Представляет базовое поле для пользовательского вычисления.|
| [base_item_position](/cells/ru/python-net/aspose.cells.pivot/pivotfield/base_item_position) | Представляет элемент в базовом поле для пользовательского расчета.<br/> Действительно только для полей данных.<br/>Поскольку PivotItemPosition.Custom предназначен только для чтения, если вам нужно установить PivotItemPosition.Custom,<br/> установите атрибут PivotField.BaseItemIndex.|
| [base_item_index](/cells/ru/python-net/aspose.cells.pivot/pivotfield/base_item_index) | Представляет элемент в базовом поле для пользовательского расчета.<br/> Действительно только для полей данных.|
| [current_page_item](/cells/ru/python-net/aspose.cells.pivot/pivotfield/current_page_item) | Представляет текущий элемент страницы, отображаемый для поля страницы (действительно только для полей страницы).|
| [number](/cells/ru/python-net/aspose.cells.pivot/pivotfield/number) | Представляет встроенный формат отображения чисел и дат.|
| [insert_blank_row](/cells/ru/python-net/aspose.cells.pivot/pivotfield/insert_blank_row) | Указывает, вставляется ли пустая строка после каждого элемента.|
| [show_subtotal_at_top](/cells/ru/python-net/aspose.cells.pivot/pivotfield/show_subtotal_at_top) | когда ShowInOutlineForm имеет значение true, промежуточные итоги отображаются вверху списка элементов, а не внизу|
| [show_in_outline_form](/cells/ru/python-net/aspose.cells.pivot/pivotfield/show_in_outline_form) | Указывает, следует ли размещать это поле в виде схемы в представлении сводной таблицы.|
| [number_format](/cells/ru/python-net/aspose.cells.pivot/pivotfield/number_format) |Представляет настраиваемый формат отображения чисел и дат.|
| [items](/cells/ru/python-net/aspose.cells.pivot/pivotfield/items) | Получить все базовые предметы;|
| [original_items](/cells/ru/python-net/aspose.cells.pivot/pivotfield/original_items) | Получить оригинальные базовые предметы;|
| [item_count](/cells/ru/python-net/aspose.cells.pivot/pivotfield/item_count) | Получает количество базовых элементов этого сводного поля.|
| [show_compact](/cells/ru/python-net/aspose.cells.pivot/pivotfield/show_compact) | Указывает, отображать ли метки из следующего поля в том же столбце в представлении сводной таблицы.|


###  Методы
| Метод| Описание|
| :- | :- |
| [hide_item(index, is_hidden)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/hide_item/#int-bool) | Устанавливает, скрыт ли конкретный PivotItem в поле данных.|
| [hide_item(item_value, is_hidden)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/hide_item/#str-bool) | Устанавливает, скрыт ли конкретный PivotItem в поле данных.|
| [get_pivot_filter_by_type(type)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/get_pivot_filter_by_type/#PivotFilterType) | Получает сводной фильтр сводного поля по типу|
| [get_pivot_filters()](/cells/ru/python-net/aspose.cells.pivot/pivotfield/get_pivot_filters/#) | Получает сводные фильтры сводного поля|
| [init_pivot_items()](/cells/ru/python-net/aspose.cells.pivot/pivotfield/init_pivot_items/#) | Инициировать элементы сводки поля сводки|
| [get_calculated_field_formula()](/cells/ru/python-net/aspose.cells.pivot/pivotfield/get_calculated_field_formula/#) | Получить строку формулы указанного вычисляемого поля.|
| [set_subtotals(subtotal_type, shown)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/set_subtotals/#PivotFieldSubtotalType-bool) | Устанавливает, показывает ли указанное поле эти промежуточные итоги.|
| [get_subtotals(subtotal_type)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/get_subtotals/#PivotFieldSubtotalType) | Получает, показывает ли указанное поле эти промежуточные итоги.|
| [is_hidden_item(index)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_hidden_item/#int) | Указывает, скрыт ли конкретный PivotItem.|
| [is_hidden_item_detail(index)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/is_hidden_item_detail/#int) | Указывает, является ли конкретный PivotItem скрытым.|
| [hide_item_detail(index, is_hidden_detail)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/hide_item_detail/#int-bool) | Устанавливает, является ли конкретный PivotItem в сводном поле скрытой деталью.|
| [hide_detail(is_hidden_detail)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/hide_detail/#bool) | Устанавливает, являются ли PivotItems в сводном поле скрытыми деталями. То есть свернуть/развернуть это поле.|
| [add_calculated_item(name, formula)](/cells/ru/python-net/aspose.cells.pivot/pivotfield/add_calculated_item/#str-str) |Добавьте вычисляемый элемент в сводное поле.|



###  Примеры

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

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
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.pivot](..)
