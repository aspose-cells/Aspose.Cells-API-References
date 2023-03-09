---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
Добавляет рабочий лист в коллекцию.


###  Возвращает

[Worksheet](/cells/ru/python-net/aspose.cells/worksheet) индекс объекта.


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
Добавляет рабочий лист в коллекцию.


###  Возвращает

[Worksheet](/cells/ru/python-net/aspose.cells/worksheet) индекс объекта.


```python
def add(self, type):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [SheetType](/cells/ru/python-net/aspose.cells/sheettype) | Тип рабочего листа.|

###  Пример

```python
from aspose.cells import SheetType, Workbook
from aspose.cells.charts import ChartType

workbook = Workbook()
workbook.worksheets.add(SheetType.CHART)
cells = workbook.worksheets[0].cells
cells.get("c2").put_value(5000)
cells.get("c3").put_value(3000)
cells.get("c4").put_value(4000)
cells.get("c5").put_value(5000)
cells.get("c6").put_value(6000)
charts = workbook.worksheets[1].charts
chartIndex = charts.add(ChartType.COLUMN, 10, 10, 20, 20)
chart = charts[chartIndex]
chart.n_series.add("Sheet1!C2:C6", True)

```


##  add(sheet_name) {#str}
Добавляет рабочий лист в коллекцию.


###  Возвращает

[Worksheet](/cells/ru/python-net/aspose.cells/worksheet) объект.


```python
def add(self, sheet_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| sheet_name | str | Имя рабочего листа|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Worksheet](/cells/ru/python-net/aspose.cells/worksheet)
* класс [WorksheetCollection](/cells/ru/python-net/aspose.cells/worksheetcollection)
