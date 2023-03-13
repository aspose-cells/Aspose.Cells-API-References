---
title: FindOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 630
url: /ru/python-net/aspose.cells/findoptions/
is_root: false
---
##  FindOptions класс
Представляет параметры поиска.



Тип FindOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [FindOptions()](/cells/ru/python-net/aspose.cells/findoptions/__init__/#) | Создает новый экземпляр FindOptions|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_case_sensitive](/cells/ru/python-net/aspose.cells/findoptions/is_case_sensitive) | Указывает, чувствительна ли искомая строка к регистру.|
| [case_sensitive](/cells/ru/python-net/aspose.cells/findoptions/case_sensitive) | Указывает, чувствительна ли искомая строка к регистру.|
| [look_at_type](/cells/ru/python-net/aspose.cells/findoptions/look_at_type) | Посмотрите на тип.|
| [is_range_set](/cells/ru/python-net/aspose.cells/findoptions/is_range_set) | Указывает, установлен ли искомый диапазон.|
| [search_next](/cells/ru/python-net/aspose.cells/findoptions/search_next) | Порядок поиска. Верно: поиск далее. False: искать предыдущий.|
| [search_backward](/cells/ru/python-net/aspose.cells/findoptions/search_backward) | Ищите ли ячейки назад.|
| [seach_order_by_rows](/cells/ru/python-net/aspose.cells/findoptions/seach_order_by_rows) | Указывает порядок поиска по строкам или столбцам.|
| [look_in_type](/cells/ru/python-net/aspose.cells/findoptions/look_in_type) | Смотри в тип.|
| [regex_key](/cells/ru/python-net/aspose.cells/findoptions/regex_key) | Указывает, является ли искомый ключ регулярным выражением.<br/>Если true, искомый ключ будет принят как регулярное выражение и проанализирован. В противном случае ключ будет проанализирован в соответствии с правилами MS Excel.|
| [value_type_sensitive](/cells/ru/python-net/aspose.cells/findoptions/value_type_sensitive) | Указывает, должен ли тип значения искомой ячейки совпадать с искомым ключом.|
| [style](/cells/ru/python-net/aspose.cells/findoptions/style) | Формат для поиска.|
| [convert_numeric_data](/cells/ru/python-net/aspose.cells/findoptions/convert_numeric_data) | Получает или задает значение, указывающее, выполняется ли преобразование искомого строкового значения в числовые данные.|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_range()](/cells/ru/python-net/aspose.cells/findoptions/get_range/#) | Получает и задает искомый диапазон.|
| [set_range(ca)](/cells/ru/python-net/aspose.cells/findoptions/set_range/#CellArea) | Устанавливает искомый диапазон.|



###  Пример

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  Смотрите также
* модуль [aspose.cells](..)
