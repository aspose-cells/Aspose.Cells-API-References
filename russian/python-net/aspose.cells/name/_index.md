---
title: Name класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1070
url: /ru/python-net/aspose.cells/name/
is_root: false
---
##  Name класс
Представляет определенное имя для диапазона ячеек.



Тип Name предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [comment](/cells/ru/python-net/aspose.cells/name/comment) | Получает и задает комментарий к имени.<br/> Применяется только для Excel 2007.|
| [text](/cells/ru/python-net/aspose.cells/name/text) | Получает текст имени объекта.|
| [full_text](/cells/ru/python-net/aspose.cells/name/full_text) | Получает полный текст имени объекта с настройкой области.|
| [refers_to](/cells/ru/python-net/aspose.cells/name/refers_to) | Возвращает или задает формулу, на которую ссылается имя, начиная со знака равенства.|
| [r1c1_refers_to](/cells/ru/python-net/aspose.cells/name/r1c1_refers_to) | Получает или задает ссылку R1C1 на [Name](/cells/ru/python-net/aspose.cells/name).|
| [is_referred](/cells/ru/python-net/aspose.cells/name/is_referred) | Указывает, используется ли это имя в других формулах.|
| [is_visible](/cells/ru/python-net/aspose.cells/name/is_visible) | Указывает, видно ли имя.|
| [sheet_index](/cells/ru/python-net/aspose.cells/name/sheet_index) | Указывает, что это имя принадлежит рабочей книге или рабочему листу.<br/> 0 = глобальное имя, в противном случае индексировать лист (на основе единицы)|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/name/get_refers_to/#bool-bool) | Получите ссылку на это имя.|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/ru/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | Получите ссылку на это имя на основе указанной ячейки.|
| [get_ranges()](/cells/ru/python-net/aspose.cells/name/get_ranges/#) |Получает все диапазоны, на которые ссылается это имя.|
| [get_ranges(recalculate)](/cells/ru/python-net/aspose.cells/name/get_ranges/#bool) |Получает все диапазоны, на которые ссылается это имя.|
| [get_range()](/cells/ru/python-net/aspose.cells/name/get_range/#) | Получает диапазон, если это имя относится к диапазону.|
| [get_range(recalculate)](/cells/ru/python-net/aspose.cells/name/get_range/#bool) | Получает диапазон, если это имя относится к диапазону|
| [get_range(sheet_index, row, column)](/cells/ru/python-net/aspose.cells/name/get_range/#int-int-int) | Получает диапазон, если это имя относится к диапазону.<br/> Если ссылка на это имя не является абсолютной, диапазон может быть разным для разных ячеек.|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/ru/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) | Установите ссылку на это имя.|
| [get_referred_areas(recalculate)](/cells/ru/python-net/aspose.cells/name/get_referred_areas/#bool) | Получает все ссылки, на которые ссылается это имя.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Name](/cells/ru/python-net/aspose.cells/name)
