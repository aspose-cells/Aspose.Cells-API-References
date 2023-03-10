---
title: AutoFilter الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter الدرجة
يمثل التصفية التلقائية لورقة العمل المحددة.



يكشف نوع AutoFilter الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [sorter](/cells/ar/python-net/aspose.cells/autofilter/sorter) | يحصل على فارز البيانات.|
| [range](/cells/ar/python-net/aspose.cells/autofilter/range) | يمثل النطاق الذي تنطبق عليه التصفية التلقائية المحددة.|
| [show_filter_button](/cells/ar/python-net/aspose.cells/autofilter/show_filter_button) | يشير إلى ما إذا كان زر التصفية التلقائية لهذا العمود مرئيًا أم لا.|
| [filter_columns](/cells/ar/python-net/aspose.cells/autofilter/filter_columns) | يحصل على مجموعة أعمدة التصفية.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/ar/python-net/aspose.cells/autofilter/remove_filter/#int-str) |يزيل عامل تصفية لعمود مرشح.|
| [remove_filter(field_index)](/cells/ar/python-net/aspose.cells/autofilter/remove_filter/#int) | قم بإزالة الفلتر المحدد.|
| [custom(field_index, operator_type1, criteria1)](/cells/ar/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | يقوم بتصفية قائمة بمعايير مخصصة.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/ar/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | يقوم بتصفية قائمة بمعايير مخصصة.|
| [refresh()](/cells/ar/python-net/aspose.cells/autofilter/refresh/#) | قم بتحديث عوامل التصفية التلقائية لإخفاء الصفوف أو إظهارها.|
| [refresh(hide_rows)](/cells/ar/python-net/aspose.cells/autofilter/refresh/#bool) | يحصل على فهارس كافة الصفوف المخفية.|
| [set_range(row, start_column, end_column)](/cells/ar/python-net/aspose.cells/autofilter/set_range/#int-int-int) | يعيّن النطاق الذي ينطبق عليه التصفية التلقائية المحددة.|
| [get_cell_area()](/cells/ar/python-net/aspose.cells/autofilter/get_cell_area/#) | الحصول على [CellArea](/cells/ar/python-net/aspose.cells/cellarea) حيث ينطبق عليه عامل التصفية التلقائي المحدد.|
| [add_filter(field_index, criteria)](/cells/ar/python-net/aspose.cells/autofilter/add_filter/#int-str) | يضيف عامل تصفية لعمود مرشح.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/ar/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | يضيف مرشح التاريخ.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/ar/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | يزيل مرشح التاريخ.|
| [filter(field_index, criteria)](/cells/ar/python-net/aspose.cells/autofilter/filter/#int-str) | يقوم بتصفية قائمة بمعايير محددة.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/ar/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | قم بتصفية أهم 10 عناصر في القائمة|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/ar/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | يضيف عامل تصفية ديناميكي.|
| [add_font_color_filter(field_index, color)](/cells/ar/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | يضيف مرشح لون الخط.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/ar/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | يضيف مرشح لون التعبئة.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/ar/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | يضيف عامل تصفية رمز.|
| [match_blanks(field_index)](/cells/ar/python-net/aspose.cells/autofilter/match_blanks/#int) | تطابق جميع الخلايا الفارغة في القائمة.|
| [match_non_blanks(field_index)](/cells/ar/python-net/aspose.cells/autofilter/match_non_blanks/#int) | تطابق جميع الخلايا غير الفارغة في القائمة.|
| [show_all()](/cells/ar/python-net/aspose.cells/autofilter/show_all/#) | إظهار كافة الصفوف.|



###  مثال

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [CellArea](/cells/ar/python-net/aspose.cells/cellarea)
