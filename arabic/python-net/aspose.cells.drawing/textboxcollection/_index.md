---
title: TextBoxCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 690
url: /ar/python-net/aspose.cells.drawing/textboxcollection/
is_root: false
---
##  TextBoxCollection الدرجة
لتغليف مجموعة من [TextBox](/cells/ar/python-net/aspose.cells.drawing/textbox) عنصر.



يكشف نوع TextBoxCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [copy_to(array)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add(upper_left_row, upper_left_column, height, width)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/add/#int-int-int-int) |يضيف مربع نص إلى المجموعة.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.drawing/textboxcollection/binary_search/#TextBox) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get collection object
textBoxCollection = workbook.worksheets[0].text_boxes
# add a textbox
textBoxCollection.add(1, 1, 50, 100)
for tbox in textBoxCollection:
    pass

```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
* فئة [TextBox](/cells/ar/python-net/aspose.cells.drawing/textbox)
