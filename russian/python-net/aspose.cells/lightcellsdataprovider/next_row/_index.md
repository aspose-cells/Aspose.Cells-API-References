---
title: next_row метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/lightcellsdataprovider/next_row/
is_root: false
---
##  next_row() {#}
Получает следующую строку для сохранения.


###  Возвращает

индекс следующей строки для сохранения. -1 означает, что достигнут конец данных текущего листа и дальнейшая строка текущего листа не может быть сохранена.


```python
def next_row(self):
    ...
```


###  Примечания

Он будет вызываться в начале сохранения данных строки и ее ячеек (до [LightCellsDataProvider.start_row(row)](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/start_row)).


###  Смотрите также

* модуль [aspose.cells](../../)
* класс [LightCellsDataProvider](/cells/ru/python-net/aspose.cells/lightcellsdataprovider)
