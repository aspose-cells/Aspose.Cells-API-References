---
title: VbaModule الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 10
url: /ar/python-net/aspose.cells.vba/vbamodule/
is_root: false
---
##  VbaModule الدرجة
يمثل الوحدة في مشروع VBA.



يكشف نوع VbaModule الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [name](/cells/ar/python-net/aspose.cells.vba/vbamodule/name) | الحصول على اسم الوحدة وتعيينه.|
| [type](/cells/ar/python-net/aspose.cells.vba/vbamodule/type) | يحصل على نوع الوحدة.|
| [codes](/cells/ar/python-net/aspose.cells.vba/vbamodule/codes) | يحصل على رموز الوحدات ويضبطها.|



###  أمثلة

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
index = vbaProject.modules.add(VbaModuleType.CLASS, "test")
#  Get vba module
vbaModule = vbaProject.modules[index]
#  Set codes
vbaModule.codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub"
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  أنظر أيضا
* وحدة [aspose.cells.vba](..)
