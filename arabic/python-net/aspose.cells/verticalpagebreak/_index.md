---
title: VerticalPageBreak الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1560
url: /ar/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  VerticalPageBreak الدرجة
لتغليف الكائن الذي يمثل فاصل صفحات عمودي.



يكشف نوع VerticalPageBreak الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [start_row](/cells/ar/python-net/aspose.cells/verticalpagebreak/start_row) | الحصول على فهرس صف البداية لفاصل الصفحات الرأسي.|
| [end_row](/cells/ar/python-net/aspose.cells/verticalpagebreak/end_row) | الحصول على فهرس صف نهاية فاصل الصفحات الرأسي.|
| [column](/cells/ar/python-net/aspose.cells/verticalpagebreak/column) | يحصل على فهرس العمود الخاص بفاصل الصفحات الرأسي.|



###  مثال

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
