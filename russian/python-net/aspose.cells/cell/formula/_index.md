---
title: formula недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 460
url: /ru/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula недвижимость

Получает или задает formula из [Cell](/cells/ru/python-net/aspose.cells/cell).

###  Примечания

 Строка formula всегда начинается со знака равенства (=).
И, пожалуйста, всегда используйте запятую (,) в качестве разделителя параметров, например "=СУММ(A1, E1, H2)".

###  Пример

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  Определение:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)
