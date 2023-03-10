---
title: SparklineGroupCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 290
url: /ar/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  SparklineGroupCollection الدرجة
لتغليف مجموعة من [SparklineGroup](/cells/ar/python-net/aspose.cells.charts/sparklinegroup) عنصر.



يكشف نوع SparklineGroupCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [copy_to(array)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add(type, data_range, is_vertical, location_range)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) | لاضافة عنصر [SparklineGroup](/cells/ar/python-net/aspose.cells.charts/sparklinegroup) للمجموعة.|
| [clear_sparklines(cell_area)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) | يمسح خطوط المؤشر الموجودة داخل منطقة من الخلايا.|
| [clear_sparkline_groups(cell_area)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) | يمسح مجموعات خط المؤشر التي تتداخل مع منطقة من الخلايا.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)

```

###  أنظر أيضا
* وحدة [aspose.cells.charts](..)
* فئة [SparklineGroup](/cells/ar/python-net/aspose.cells.charts/sparklinegroup)
