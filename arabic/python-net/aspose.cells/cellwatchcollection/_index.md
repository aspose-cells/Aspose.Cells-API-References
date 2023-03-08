---
title: CellWatchCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 170
url: /ar/python-net/aspose.cells/cellwatchcollection/
is_root: false
---
##  CellWatchCollection الدرجة
يمثل مجموعة الخلايا الموجودة في ورقة العمل هذه والتي يتم مشاهدتها في "نافذة المراقبة".



يكشف نوع CellWatchCollection الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [CellWatchCollection()](/cells/ar/python-net/aspose.cells/cellwatchcollection/__init__/#) |إنشاء مثيل جديد من CellWatchCollection|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells/cellwatchcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(row, column)](/cells/ar/python-net/aspose.cells/cellwatchcollection/add/#int-int) | اضافة [CellWatch](/cells/ar/python-net/aspose.cells/cellwatch) بالصف والعمود.|
| [add(cell_name)](/cells/ar/python-net/aspose.cells/cellwatchcollection/add/#str) | إضافة [CellWatch](/cells/ar/python-net/aspose.cells/cellwatch) باسم الخلية.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells/cellwatchcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells/cellwatchcollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells/cellwatchcollection/binary_search/#CellWatch) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet.
sheet = workbook.worksheets[0]
#  Add Cell Watch Item into the watch window
sheet.cell_watches.add("B2")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [CellWatch](/cells/ar/python-net/aspose.cells/cellwatch)
