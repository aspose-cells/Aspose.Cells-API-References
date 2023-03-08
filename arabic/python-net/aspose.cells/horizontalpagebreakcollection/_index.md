---
title: HorizontalPageBreakCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 760
url: /ar/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection الدرجة
لتغليف مجموعة من [HorizontalPageBreak](/cells/ar/python-net/aspose.cells/horizontalpagebreak) عنصر.



يكشف نوع HorizontalPageBreakCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(row, start_column, end_column)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | يضيف فاصل صفحات أفقيًا إلى المجموعة.|
| [add(row)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | يضيف فاصل صفحات أفقيًا إلى المجموعة.|
| [add(row, column)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | يضيف فاصل صفحات أفقيًا إلى المجموعة.|
| [add(cell_name)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | يضيف فاصل صفحات أفقيًا إلى المجموعة.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



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
* فئة [HorizontalPageBreak](/cells/ar/python-net/aspose.cells/horizontalpagebreak)
