---
title: طريقة get_enumerator
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 90
url: /ar/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
الحصول على عداد الخلايا في هذا النطاق.


###  عائدات

عداد الخلايا


```python
def get_enumerator(self):
    ...
```


###  ملاحظات

عند اجتياز العناصر بواسطة Enumerator المرتجع ، فإن مجموعة الخلايا
لا ينبغي تعديله (مثل العمليات التي ستؤدي إلى إنشاء نسخة جديدة من Cell / صف أو حذف Cell الموجود / الصف).
وإلا فقد لا يتمكن العداد من اجتياز جميع الخلايا بشكل صحيح (قد يتم اجتياز بعض العناصر بشكل متكرر أو تخطيها).
###  أمثلة

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Range](/cells/ar/python-net/aspose.cells/range)
