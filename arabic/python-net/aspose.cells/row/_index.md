---
title: Row الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1300
url: /ar/python-net/aspose.cells/row/
is_root: false
---
##  Row الدرجة
يمثل صفًا واحدًا في ورقة عمل.



يكشف نوع Row الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_blank](/cells/ar/python-net/aspose.cells/row/is_blank) | يشير إلى ما إذا كان الصف يحتوي على أية بيانات|
| [is_collapsed](/cells/ar/python-net/aspose.cells/row/is_collapsed) | ما إذا كان الصف مطويًا أم لا|
| [height](/cells/ar/python-net/aspose.cells/row/height) | الحصول على ارتفاع الصف وتعيينه بوحدات من النقاط.|
| [is_hidden](/cells/ar/python-net/aspose.cells/row/is_hidden) | يشير إلى ما إذا كان الصف مخفيًا.|
| [index](/cells/ar/python-net/aspose.cells/row/index) | يحصل على فهرس هذا الصف.|
| [group_level](/cells/ar/python-net/aspose.cells/row/group_level) | يحصل على مستوى المجموعة للصف.|
| [is_height_matched](/cells/ar/python-net/aspose.cells/row/is_height_matched) |يشير إلى تطابق ارتفاع الصف وارتفاع الخط الافتراضي.|
| [style](/cells/ar/python-net/aspose.cells/row/style) | يمثل نمط هذا الصف.|
| [has_custom_style](/cells/ar/python-net/aspose.cells/row/has_custom_style) | يشير إلى ما إذا كان هذا الصف يحتوي على إعدادات نمط مخصصة (تختلف عن الإعداد الافتراضي الموروث من المصنف).|
| [first_cell](/cells/ar/python-net/aspose.cells/row/first_cell) | الحصول على أول كائن خلية في الصف.|
| [first_data_cell](/cells/ar/python-net/aspose.cells/row/first_data_cell) | الحصول على أول خلية غير فارغة في الصف.|
| [last_cell](/cells/ar/python-net/aspose.cells/row/last_cell) | الحصول على آخر كائن خلية في الصف.|
| [last_data_cell](/cells/ar/python-net/aspose.cells/row/last_data_cell) | الحصول على آخر خلية غير فارغة في الصف.|



يحصل على الخلية.
###  مفهرس
| اسم| وصف|
| :- | :- |
| [index] | فهرس العمود|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [get_cell_by_index(index)](/cells/ar/python-net/aspose.cells/row/get_cell_by_index/#int) | احصل على الخلية حسب فهرس محدد في القائمة.|
| [get_cell_or_null(column)](/cells/ar/python-net/aspose.cells/row/get_cell_or_null/#int) | الحصول على الخلية أو القيمة الخالية في الفهرس المحدد.|
| [get_style()](/cells/ar/python-net/aspose.cells/row/get_style/#) | يحصل على نمط هذا الصف.|
| [set_style(style)](/cells/ar/python-net/aspose.cells/row/set_style/#Style) | يحدد نمط هذا الصف.|
| [copy_settings(source, check_style)](/cells/ar/python-net/aspose.cells/row/copy_settings/#Row-bool) | نسخ إعدادات الصف ، مثل النمط ، الارتفاع ، الرؤية ، ... إلخ.|
| [apply_style(style, flag)](/cells/ar/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | يطبق التنسيقات على صف كامل.|
| [equals(row)](/cells/ar/python-net/aspose.cells/row/equals/#Row) | للتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع كائن صف آخر.|



###  أمثلة

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
