---
title: start_row метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Начинает сохранять данные одной строки.



```python
def start_row(self, row):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| row | [Row](/cells/ru/python-net/aspose.cells/row) | Объект строки для реализации для заполнения данных. Его индекс строки — это возвращаемое значение последнего вызова [LightCellsDataProvider.next_row()](/cells/ru/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>Если строка была инициализирована во внутренней модели ячеек, будет использоваться существующий объект строки.<br/> В противном случае для реализации будет использоваться временный объект Row для заполнения данных.|
###  Примечания

Он будет вызываться в начале сохранения данных строки и ее ячеек.
Если текущая строка имеет некоторые настраиваемые свойства, такие как высота, стиль и т. д.,
реализация должна установить эти свойства для данного объекта Row здесь.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [LightCellsDataProvider](/cells/ru/python-net/aspose.cells/lightcellsdataprovider)
