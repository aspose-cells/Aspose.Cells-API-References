---
title: ColumnCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 270
url: /ar/python-net/aspose.cells/columncollection/
is_root: false
---
##  ColumnCollection الدرجة
مجموعة من [Column](/cells/ar/python-net/aspose.cells/column) كائنات تمثل الأعمدة الفردية (الإعدادات) في ورقة العمل.
يمثل كائن العمود فقط الإعدادات مثل عرض العمود والأنماط وما إلى ذلك. للعمود بأكمله ،
لا علاقة له بحقيقة وجود خلايا (بيانات) غير فارغة أو عدم وجودها في العمود المقابل.
ويمثل "العدد" لهذه المجموعة فقط كائنات عمود العد التي تم إنشاء مثيل لها في هذه المجموعة ،
لا علاقة له بحقيقة وجود خلايا (بيانات) غير فارغة أو عدم وجودها في ورقة العمل.



يكشف نوع ColumnCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells/columncollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [copy_to(array)](/cells/ar/python-net/aspose.cells/columncollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells/columncollection/index_of/#Column-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells/columncollection/last_index_of/#Column) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells/columncollection/last_index_of/#Column-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [get_by_index(index)](/cells/ar/python-net/aspose.cells/columncollection/get_by_index/#int) | يحصل على كائن العمود بالفهرس.|
| [get_column_by_index(index)](/cells/ar/python-net/aspose.cells/columncollection/get_column_by_index/#int) | يحصل على العنصر [Column](/cells/ar/python-net/aspose.cells/column) من خلال الموضع في الكشف.|
| [binary_search(item)](/cells/ar/python-net/aspose.cells/columncollection/binary_search/#Column) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  مثال

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [Column](/cells/ar/python-net/aspose.cells/column)
