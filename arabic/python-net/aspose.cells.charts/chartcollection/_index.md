---
title: ChartCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 50
url: /ar/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection الدرجة
لتغليف مجموعة من [Chart](/cells/ar/python-net/aspose.cells.charts/chart) عنصر.



يكشف نوع ChartCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.charts/chartcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/ar/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | يضيف مخططًا إلى المجموعة.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/ar/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | يضيف مخططًا إلى المجموعة.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/ar/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | يضيف مخططًا بقالب محدد مسبقًا.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/ar/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | يضيف مخططًا إلى المجموعة.|
| [get(index)](/cells/ar/python-net/aspose.cells.charts/chartcollection/get/#int) |أضف API for Python عبر .Net. لأن هذا [الفهرس] غير مدعوم|
| [get(name)](/cells/ar/python-net/aspose.cells.charts/chartcollection/get/#str) | أضف API for Python عبر .Net. نظرًا لأن [مخطط السلسلة] هذا غير مدعوم|
| [copy_to(array)](/cells/ar/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add_floating_chart(type, left, top, width, height)](/cells/ar/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | يضيف مخططًا إلى المجموعة.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  أنظر أيضا
* وحدة [aspose.cells.charts](..)
* فئة [Chart](/cells/ar/python-net/aspose.cells.charts/chart)
