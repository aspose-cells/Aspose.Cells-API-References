---
title: CheckBoxCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 100
url: /ar/python-net/aspose.cells.drawing/checkboxcollection/
is_root: false
---
##  CheckBoxCollection الدرجة
يمثل مجموعة من [CheckBox](/cells/ar/python-net/aspose.cells.drawing/checkbox) كائنات في ورقة عمل.



يكشف نوع CheckBoxCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [copy_to(array)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/index_of/#CheckBox-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/index_of/#CheckBox-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/last_index_of/#CheckBox) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/last_index_of/#CheckBox-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/last_index_of/#CheckBox-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [add(upper_left_row, upper_left_column, height, width)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/add/#int-int-int-int) | يضيف خانة اختيار إلى المجموعة.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.drawing/checkboxcollection/binary_search/#CheckBox) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet in the workbook.
sheet = workbook.worksheets[0]
index = sheet.check_boxes.add(15, 15, 20, 100)
checkBox = sheet.check_boxes[index]
checkBox.text = "Check Box 1"

```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
* فئة [CheckBox](/cells/ar/python-net/aspose.cells.drawing/checkbox)
