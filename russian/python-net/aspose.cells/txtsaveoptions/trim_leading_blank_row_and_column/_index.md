---
title: trim_leading_blank_row_and_column недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 220
url: /ru/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
##  trim_leading_blank_row_and_column недвижимость

Указывает, следует ли обрезать ведущие пустые строки и столбцы, как это делает MS Excel.
Значение по умолчанию верно.

###  Примечания

То же самое с правилом в MS Excel: строка/столбец не будет восприниматься как пустая, если она имеет собственный стиль,
даже если он не содержит данных ячейки.
При сохранении в режиме LightCells этот параметр не действует.
Пользователь должен контролировать выходной диапазон с помощью реализации [TxtSaveOptions.light_cells_data_provider](/cells/ru/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider).
или набрав [TxtSaveOptions.export_area](/cells/ru/python-net/aspose.cells/txtsaveoptions#export_area)
###  Определение:
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [TxtSaveOptions](/cells/ru/python-net/aspose.cells/txtsaveoptions)
