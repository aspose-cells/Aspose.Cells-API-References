---
title: add_active_x_control yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
Bir Activex Denetimi oluşturur.


###  İadeler




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | Denetimin türü.|
| top_row | int | Sol üst sıra dizini.|
| top | int | Shape öğesinin sol satırından dikey uzaklığını piksel birimi cinsinden temsil eder.|
| left_column | int | Sol üst sütun dizini.|
| left | int | Shape'in sol sütunundan yatay uzaklığını piksel birimi cinsinden temsil eder.|
| width | int | Şeklin genişliğini piksel cinsinden temsil eder.|
| height | int | Şeklin yüksekliğini piksel birimleri cinsinden temsil eder.|

###  örnekler

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)
