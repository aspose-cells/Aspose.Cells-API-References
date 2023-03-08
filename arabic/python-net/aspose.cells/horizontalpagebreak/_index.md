---
title: HorizontalPageBreak الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 750
url: /ar/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  HorizontalPageBreak الدرجة
لتغليف الكائن الذي يمثل فاصل صفحات أفقيًا.



يكشف نوع HorizontalPageBreak الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [start_column](/cells/ar/python-net/aspose.cells/horizontalpagebreak/start_column) | الحصول على فهرس عمود البداية لفاصل الصفحات الأفقي هذا.|
| [end_column](/cells/ar/python-net/aspose.cells/horizontalpagebreak/end_column) |يحصل على فهرس عمود نهاية فاصل الصفحات الأفقي هذا.|
| [row](/cells/ar/python-net/aspose.cells/horizontalpagebreak/row) | يحصل على فهرس الصف الصفري.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
