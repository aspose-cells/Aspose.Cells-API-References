---
title: VbaProjectReference الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  VbaProjectReference الدرجة
يمثل مرجع مشروع VBA.



يكشف نوع VbaProjectReference الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [type](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/type) | يحصل على نوع هذا المرجع.|
| [name](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/name) | الحصول على اسم المرجع وتعيينه.|
| [libid](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/libid) | الحصول على وتعيين Libid الخاص بالمرجع.|
| [twiddledlibid](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | الحصول على وتعيين الفهرس الملتوي للمرجع.|
| [extended_libid](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | الحصول على وتعيين Libid الموسع للمرجع.|
| [relative_libid](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) | الحصول على معرف مشروع VBA المشار إليه مع مسار نسبي وتعيينه.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [copy(source)](/cells/ar/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  أنظر أيضا
* وحدة [aspose.cells.vba](..)
