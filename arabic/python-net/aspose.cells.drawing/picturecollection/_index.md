---
title: PictureCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 460
url: /ar/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection الدرجة
لتغليف مجموعة من [Picture](/cells/ar/python-net/aspose.cells.drawing/picture) عنصر.



يكشف نوع PictureCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.drawing/picturecollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | يضيف صورة إلى المجموعة.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | يضيف صورة إلى المجموعة.|
| [add(upper_left_row, upper_left_column, stream)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | يضيف صورة إلى المجموعة.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | يضيف صورة إلى المجموعة.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | يضيف صورة إلى المجموعة.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | يضيف صورة إلى المجموعة.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
* فئة [Picture](/cells/ar/python-net/aspose.cells.drawing/picture)
