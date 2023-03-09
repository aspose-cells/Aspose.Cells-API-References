---
title: PivotTableCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 110
url: /ar/python-net/aspose.cells.pivot/pivottablecollection/
is_root: false
---
##  PivotTableCollection الدرجة
يمثل مجموعة كل كائنات PivotTable في ورقة العمل المحددة.



يكشف نوع PivotTableCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [capacity](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/capacity) | الحصول على أو تحديد عدد العناصر التي يمكن أن تحتويها قائمة الصفيف.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(source_data, dest_cell_name, table_name)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.|
| [add(source_data, dest_cell_name, table_name, use_same_source)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str-bool) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.|
| [add(source_data, row, column, table_name)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.|
| [add(source_data, row, column, table_name, use_same_source)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str-bool) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.|
| [add(pivot_table, dest_cell_name, table_name)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-str-str) | إضافة كائن PivotTable جديد إلى المجموعة من PivotTable آخر.|
| [add(pivot_table, row, column, table_name)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-int-int-str) | إضافة كائن PivotTable جديد إلى المجموعة من PivotTable آخر.|
| [add(source_data, is_auto_page, page_fields, dest_cell_name, table_name)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-str-str) | يضيف كائن PivotTable جديدًا إلى المجموعة ذات نطاقات الدمج المتعددة كمصدر بيانات.|
| [add(source_data, is_auto_page, page_fields, row, column, table_name)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-int-int-str) | يضيف كائن PivotTable جديدًا إلى المجموعة ذات نطاقات الدمج المتعددة كمصدر بيانات.|
| [copy_to(array)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | ينسخ قائمة المصفوفات بأكملها إلى قائمة مصفوفة متوافقة أحادية البعد ، بدءًا من بداية قائمة الصفيف الهدف.|
| [copy_to(index, array, array_index, count)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) |ينسخ نطاقًا من العناصر من قائمة المصفوفة إلى قائمة مصفوفة أحادية البعد متوافقة ، بدءًا من الفهرس المحدد لقائمة الصفيف الهدف.|
| [index_of(item, index)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من الفهرس المحدد إلى العنصر الأخير.|
| [index_of(item, index, count)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int-int) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأول ضمن نطاق العناصر في قائمة الصفيف الذي يبدأ بالفهرس المحدد ويحتوي على عدد محدد من العناصر.|
| [last_index_of(item)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable) | البحث عن الكائن المحدد وإرجاع الفهرس الصفري للتواجد الأخير ضمن قائمة الصفيف بأكملها.|
| [last_index_of(item, index)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int) | يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف الذي يمتد من العنصر الأول إلى الفهرس المحدد.|
| [last_index_of(item, index, count)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int-int) |يبحث عن الكائن المحدد ويعيد الفهرس الصفري للتواجد الأخير ضمن نطاق العناصر في قائمة الصفيف التي تحتوي على عدد محدد من العناصر وتنتهي عند الفهرس المحدد.|
| [remove_at(index, keep_data)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | يحذف PivotTable في الفهرس المحدد|
| [binary_search(item)](/cells/ar/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#PivotTable) | يبحث في قائمة الصفيف التي تم فرزها بالكامل عن عنصر باستخدام المقارنة الافتراضية ويعيد فهرس العنصر على أساس الصفر.|



###  أمثلة

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells.pivot](..)
