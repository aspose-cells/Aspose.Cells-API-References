---
title: formula mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 460
url: /tr/python-net/aspose.cells/cell/formula/
is_root: false
---
##  formula mülk

[Cell](/cells/tr/python-net/aspose.cells/cell)'in formula'ini alır veya ayarlar.

###  Notlar

 formula dizesi her zaman eşittir işaretiyle (=) başlar.
Ve lütfen "=SUM(A1, E1, H2)" gibi parametre ayırıcı olarak her zaman virgül(,) kullanın.

###  Örnek

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
###  Tanım:
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
