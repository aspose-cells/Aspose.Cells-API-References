---
title: Range الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1250
url: /ar/python-net/aspose.cells/range/
is_root: false
---
##  Range الدرجة
لتغليف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول بيانات.



يكشف نوع Range الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [current_region](/cells/ar/python-net/aspose.cells/range/current_region) |إرجاع كائن النطاق الذي يمثل المنطقة الحالية.<br/> المنطقة الحالية عبارة عن نطاق يحده أي مجموعة من الصفوف الفارغة والأعمدة الفارغة.|
| [hyperlinks](/cells/ar/python-net/aspose.cells/range/hyperlinks) | يحصل على كل الارتباط التشعبي في النطاق.|
| [row_count](/cells/ar/python-net/aspose.cells/range/row_count) | الحصول على عدد الصفوف في النطاق.|
| [column_count](/cells/ar/python-net/aspose.cells/range/column_count) | الحصول على عدد الأعمدة في النطاق.|
| [cell_count](/cells/ar/python-net/aspose.cells/range/cell_count) | الحصول على كل عدد الخلايا في النطاق.|
| [name](/cells/ar/python-net/aspose.cells/range/name) | الحصول على أو تحديد اسم النطاق.|
| [refers_to](/cells/ar/python-net/aspose.cells/range/refers_to) | يحصل على النطاق الذي يشير إليه.|
| [address](/cells/ar/python-net/aspose.cells/range/address) | يحصل على عنوان النطاق.|
| [left](/cells/ar/python-net/aspose.cells/range/left) | الحصول على المسافة ، بالنقاط ، من الحافة اليسرى للعمود A إلى الحافة اليسرى من النطاق.|
| [top](/cells/ar/python-net/aspose.cells/range/top) | الحصول على المسافة ، بالنقاط ، من الحافة العلوية للصف 1 إلى الحافة العلوية من النطاق.|
| [width](/cells/ar/python-net/aspose.cells/range/width) | الحصول على عرض النطاق بالنقاط.|
| [height](/cells/ar/python-net/aspose.cells/range/height) | الحصول على عرض النطاق بالنقاط.|
| [first_row](/cells/ar/python-net/aspose.cells/range/first_row) | الحصول على فهرس الصف الأول من النطاق.|
| [first_column](/cells/ar/python-net/aspose.cells/range/first_column) | الحصول على فهرس العمود الأول من النطاق.|
| [value](/cells/ar/python-net/aspose.cells/range/value) | الحصول على قيمة النطاق وتعيينها.|
| [column_width](/cells/ar/python-net/aspose.cells/range/column_width) | تعيين عرض العمود لهذا النطاق أو الحصول عليه|
| [row_height](/cells/ar/python-net/aspose.cells/range/row_height) | تعيين أو الحصول على ارتفاع الصفوف في هذا النطاق|
| [entire_column](/cells/ar/python-net/aspose.cells/range/entire_column) |الحصول على كائن Range يمثل العمود (أو الأعمدة) بأكمله الذي يحتوي على النطاق المحدد.|
| [entire_row](/cells/ar/python-net/aspose.cells/range/entire_row) | الحصول على كائن Range يمثل الصف بأكمله (أو الصفوف) الذي يحتوي على النطاق المحدد.|
| [worksheet](/cells/ar/python-net/aspose.cells/range/worksheet) | الحصول على الكائن [Range.worksheet](/cells/ar/python-net/aspose.cells/range#worksheet) الذي يحتوي على هذا النطاق.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [auto_fill(target)](/cells/ar/python-net/aspose.cells/range/auto_fill/#Range) | كل ملء النطاق المستهدف.|
| [auto_fill(target, auto_fill_type)](/cells/ar/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | كل ملء النطاق المستهدف.|
| [set_style(style, explicit_flag)](/cells/ar/python-net/aspose.cells/range/set_style/#Style-bool) | قم بتطبيق نمط الخلية.|
| [set_style(style)](/cells/ar/python-net/aspose.cells/range/set_style/#Style) | يعيّن نمط النطاق.|
| [set_outline_borders(border_style, border_color)](/cells/ar/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | يضبط حدود المخطط التفصيلي حول نطاق من الخلايا بنفس نمط ولون الحدود.|
| [set_outline_borders(border_style, border_color)](/cells/ar/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | يضبط حدود المخطط التفصيلي حول نطاق من الخلايا بنفس نمط ولون الحدود.|
| [set_outline_borders(border_styles, border_colors)](/cells/ar/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | يحدد حدود الخط حول نطاق من الخلايا.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/ar/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | يعين حدود المخطط التفصيلي حول نطاق من الخلايا.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/ar/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | يعين حدود المخطط التفصيلي حول نطاق من الخلايا.|
| [copy(range, options)](/cells/ar/python-net/aspose.cells/range/copy/#Range-PasteOptions) | نسخ النطاق مع خيارات لصق خاصة.|
| [copy(range)](/cells/ar/python-net/aspose.cells/range/copy/#Range) | ينسخ البيانات (بما في ذلك الصيغ) والتنسيق ورسم الكائنات وما إلى ذلك من نطاق المصدر.|
| [get_enumerator()](/cells/ar/python-net/aspose.cells/range/get_enumerator/#) | الحصول على عداد الخلايا في هذا النطاق.|
| [is_intersect(range)](/cells/ar/python-net/aspose.cells/range/is_intersect/#Range) | يشير إلى ما إذا كان النطاق متقاطعًا.|
| [intersect(range)](/cells/ar/python-net/aspose.cells/range/intersect/#Range) | إرجاع عنصر [Range](/cells/ar/python-net/aspose.cells/range) يمثل التقاطع المستطيل لنطاقين.|
| [union(range)](/cells/ar/python-net/aspose.cells/range/union/#Range) | تُرجع اتحاد نطاقين.|
| [merge()](/cells/ar/python-net/aspose.cells/range/merge/#) | يدمج نطاقًا من الخلايا في خلية واحدة.|
| [un_merge()](/cells/ar/python-net/aspose.cells/range/un_merge/#) |يدمج الخلايا المدمجة من هذا النطاق.|
| [put_value(string_value, is_converted, set_style)](/cells/ar/python-net/aspose.cells/range/put_value/#str-bool-bool) | يضع قيمة في النطاق ، إذا كان ذلك مناسبًا ، فسيتم تحويل القيمة إلى نوع بيانات آخر وستتم إعادة تعيين تنسيق رقم الخلية.|
| [apply_style(style, flag)](/cells/ar/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | يطبق التنسيقات على نطاق كامل.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/ar/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | تعيين الحدود الداخلية للنطاق.|
| [move_to(dest_row, dest_column)](/cells/ar/python-net/aspose.cells/range/move_to/#int-int) | انقل النطاق الحالي إلى نطاق التوزيع المباشر.|
| [copy_data(range)](/cells/ar/python-net/aspose.cells/range/copy_data/#Range) | ينسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق مصدر.|
| [copy_value(range)](/cells/ar/python-net/aspose.cells/range/copy_value/#Range) | ينسخ قيمة الخلية من نطاق المصدر.|
| [copy_style(range)](/cells/ar/python-net/aspose.cells/range/copy_style/#Range) | ينسخ إعدادات النمط من نطاق المصدر.|
| [get_cell_or_null(row_offset, column_offset)](/cells/ar/python-net/aspose.cells/range/get_cell_or_null/#int-int) | الحصول على عنصر [Cell](/cells/ar/python-net/aspose.cells/cell) أو الحصول على قيمة خالية في هذا النطاق.|
| [get_offset(row_offset, column_offset)](/cells/ar/python-net/aspose.cells/range/get_offset/#int-int) | الحصول على نطاق [Range](/cells/ar/python-net/aspose.cells/range) عن طريق الإزاحة.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)
* فئة [Range](/cells/ar/python-net/aspose.cells/range)
