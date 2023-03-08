---
title: CellArea الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 150
url: /ar/python-net/aspose.cells/cellarea/
is_root: false
---
##  CellArea الدرجة
تمثل منطقة من الخلايا.



يكشف نوع CellArea الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [CellArea()](/cells/ar/python-net/aspose.cells/cellarea/__init__/#) | ينشئ مثيلاً جديدًا من CellArea|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [start_row](/cells/ar/python-net/aspose.cells/cellarea/start_row) | الحصول على صف البداية لهذه المنطقة أو تعيينه.|
| [end_row](/cells/ar/python-net/aspose.cells/cellarea/end_row) | الحصول على صف نهاية هذه المنطقة أو تعيينه.|
| [start_column](/cells/ar/python-net/aspose.cells/cellarea/start_column) | الحصول على أو تعيين عمود البداية لهذه المنطقة.|
| [end_column](/cells/ar/python-net/aspose.cells/cellarea/end_column) | الحصول على عمود نهاية هذه المنطقة أو تعيينه.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/ar/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | ينشئ منطقة خلية.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/ar/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | ينشئ منطقة خلية.|
| [compare_to(obj)](/cells/ar/python-net/aspose.cells/cellarea/compare_to/#any) | قارن بين كائنين من نوع CellArea وفقًا للزاوية العلوية اليسرى.|



###  مثال

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
