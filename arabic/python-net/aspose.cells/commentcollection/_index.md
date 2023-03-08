---
title: CommentCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 290
url: /ar/python-net/aspose.cells/commentcollection/
is_root: false
---
##  CommentCollection الدرجة
لتغليف مجموعة من [Comment](/cells/ar/python-net/aspose.cells/comment) عنصر.



يكشف نوع CommentCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells/commentcollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/ar/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | يضيف تعليق مترابط.|
| [add_threaded_comment(cell_name, text, author)](/cells/ar/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | يضيف تعليق مترابط.|
| [get_threaded_comments(row, column)](/cells/ar/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | الحصول على التعليقات المترابطة حسب فهرس الصف والعمود.|
| [get_threaded_comments(cell_name)](/cells/ar/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | يحصل على التعليقات المترابطة حسب اسم الخلية.|
| [add(row, column)](/cells/ar/python-net/aspose.cells/commentcollection/add/#int-int) | يضيف تعليقًا إلى المجموعة.|
| [add(cell_name)](/cells/ar/python-net/aspose.cells/commentcollection/add/#str) | يضيف تعليقًا إلى المجموعة.|
| [remove_at(cell_name)](/cells/ar/python-net/aspose.cells/commentcollection/remove_at/#str) | يزيل تعليق الخلية المحددة.|
| [remove_at(row, column)](/cells/ar/python-net/aspose.cells/commentcollection/remove_at/#int-int) | يزيل تعليق الخلية المحددة.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells/commentcollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) | ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells/commentcollection/binary_search/#Comment) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [Comment](/cells/ar/python-net/aspose.cells/comment)
