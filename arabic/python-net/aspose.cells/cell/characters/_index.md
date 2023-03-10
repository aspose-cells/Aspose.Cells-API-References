---
title: طريقة characters
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells/cell/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
تقوم بإرجاع عنصر أحرف يمثل نطاقًا من characters داخل نص الخلية.


###  عائدات

كائن الأحرف.


```python
def characters(self, start_index, length):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| start_index | int | فهرس بداية الحرف.|
| length | int | عدد الأحرف.|
###  ملاحظات

تعمل هذه الطريقة فقط على الخلية ذات قيمة السلسلة.
###  مثال


```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)
