---
title: VbaModuleCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.vba/vbamodulecollection/
is_root: false
---
##  VbaModuleCollection الدرجة
تمثل قائمة [VbaModule](/cells/ar/python-net/aspose.cells.vba/vbamodule)



يكشف نوع VbaModuleCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(sheet)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/add/#Worksheet) | يضيف وحدة لورقة العمل.|
| [add(type, name)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/add/#VbaModuleType-str) | يضيف وحدة.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add_designer_storage(name, data)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/add_designer_storage/#str-bytes) |  |
| [get_designer_storage(name)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/get_designer_storage/#str) | يمثل بيانات المصمم.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.vba/vbamodulecollection/binary_search/#VbaModule) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
vbaProject.modules.add(VbaModuleType.CLASS, "test")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  أنظر أيضا
* وحدة [aspose.cells.vba](..)
* فئة [VbaModule](/cells/ar/python-net/aspose.cells.vba/vbamodule)
