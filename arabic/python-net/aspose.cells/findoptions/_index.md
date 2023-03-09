---
title: FindOptions الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 630
url: /ar/python-net/aspose.cells/findoptions/
is_root: false
---
##  FindOptions الدرجة
يمثل خيارات البحث.



يكشف نوع FindOptions الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [FindOptions()](/cells/ar/python-net/aspose.cells/findoptions/__init__/#) | إنشاء مثيل جديد لـ FindOptions|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_case_sensitive](/cells/ar/python-net/aspose.cells/findoptions/is_case_sensitive) | يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف.|
| [case_sensitive](/cells/ar/python-net/aspose.cells/findoptions/case_sensitive) | يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف.|
| [look_at_type](/cells/ar/python-net/aspose.cells/findoptions/look_at_type) | انظر إلى النوع.|
| [is_range_set](/cells/ar/python-net/aspose.cells/findoptions/is_range_set) | يشير إلى ما إذا كان النطاق الذي تم البحث عنه قد تم تعيينه.|
| [search_next](/cells/ar/python-net/aspose.cells/findoptions/search_next) | ترتيب البحث صواب: البحث التالي خطأ: البحث السابق.|
| [search_backward](/cells/ar/python-net/aspose.cells/findoptions/search_backward) | سواء كان البحث للخلف عن الخلايا.|
| [seach_order_by_rows](/cells/ar/python-net/aspose.cells/findoptions/seach_order_by_rows) | يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة.|
| [look_in_type](/cells/ar/python-net/aspose.cells/findoptions/look_in_type) | ابحث في النوع.|
| [regex_key](/cells/ar/python-net/aspose.cells/findoptions/regex_key) | يشير إلى ما إذا كان المفتاح الذي تم البحث عنه هو regex أم لا.<br/>إذا كان هذا صحيحًا ، فسيتم اعتبار المفتاح الذي تم البحث عنه كـ regex وتحليله.|
| [value_type_sensitive](/cells/ar/python-net/aspose.cells/findoptions/value_type_sensitive) | يشير إلى ما إذا كان يجب أن يكون نوع قيمة الخلية التي تم البحث عنها هو نفسه مع المفتاح الذي تم البحث عنه.|
| [style](/cells/ar/python-net/aspose.cells/findoptions/style) | التنسيق المطلوب البحث عنه.|
| [convert_numeric_data](/cells/ar/python-net/aspose.cells/findoptions/convert_numeric_data) | الحصول على أو تعيين قيمة تشير إلى ما إذا كان سيتم تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [get_range()](/cells/ar/python-net/aspose.cells/findoptions/get_range/#) | يحصل ويضبط النطاق الذي تم البحث فيه.|
| [set_range(ca)](/cells/ar/python-net/aspose.cells/findoptions/set_range/#CellArea) | يحدد النطاق الذي تم البحث عنه.|



###  أمثلة

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
