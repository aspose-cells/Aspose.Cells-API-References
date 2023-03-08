---
title: ValidationCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1550
url: /ar/python-net/aspose.cells/validationcollection/
is_root: false
---
##  ValidationCollection الدرجة
يمثل جمع التحقق من صحة البيانات.



يكشف نوع ValidationCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells/validationcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add()](/cells/ar/python-net/aspose.cells/validationcollection/add/#) | يضيف التحقق من صحة البيانات إلى المجموعة.|
| [add(ca)](/cells/ar/python-net/aspose.cells/validationcollection/add/#CellArea) | يضيف التحقق من صحة البيانات إلى المجموعة.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells/validationcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [remove_a_cell(row, column)](/cells/ar/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | يزيل كل إعدادات التحقق من صحة الخلية.|
| [remove_area(ca)](/cells/ar/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | يزيل كل إعدادات التحقق من النطاق ..|
| [get_validation_in_cell(row, column)](/cells/ar/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | يحصل على التحقق المطبق على خلية معينة.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells/validationcollection/binary_search/#Validation) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
