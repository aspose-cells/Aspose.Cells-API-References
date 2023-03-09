---
title: is_gather_string метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Проверяет, нужно ли собирать текущее строковое значение ячейки в глобальный пул.


###  Возвращает

Значение true, если строковое значение необходимо собрать в глобальный пул для результирующего файла.


```python
def is_gather_string(self):
    ...
```


###  Примечания

Сбор строковых значений будет полезен только тогда, когда для ячеек, предоставляемых этой реализацией, имеется много повторяющихся строковых значений.
В этой ситуации сбор строки сэкономит много памяти и создаст результирующий файл меньшего размера.
Если имеется много строковых значений для ячеек, предоставляемых LightCellsDataProvider, но лишь немногие из них совпадают,
сбор строки будет стоить больше памяти и времени и не будет иметь преимуществ для результирующего файла.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [LightCellsDataProvider](/cells/ru/python-net/aspose.cells/lightcellsdataprovider)
