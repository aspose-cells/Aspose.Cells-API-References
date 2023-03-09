---
title: Name الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1070
url: /ar/python-net/aspose.cells/name/
is_root: false
---
##  Name الدرجة
يمثل اسمًا محددًا لنطاق من الخلايا.



يكشف نوع Name الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [comment](/cells/ar/python-net/aspose.cells/name/comment) | الحصول على تعليق الاسم وتعيينه.<br/> ينطبق فقط على Excel 2007.|
| [text](/cells/ar/python-net/aspose.cells/name/text) | يحصل على اسم نص الكائن.|
| [full_text](/cells/ar/python-net/aspose.cells/name/full_text) | الحصول على اسم النص الكامل للكائن مع إعداد النطاق.|
| [refers_to](/cells/ar/python-net/aspose.cells/name/refers_to) | إرجاع أو تعيين الصيغة التي تم تعريف الاسم للإشارة إليها ، بدءًا بعلامة التساوي.|
| [r1c1_refers_to](/cells/ar/python-net/aspose.cells/name/r1c1_refers_to) | الحصول على أو تحديد مرجع R1C1 للرقم [Name](/cells/ar/python-net/aspose.cells/name).|
| [is_referred](/cells/ar/python-net/aspose.cells/name/is_referred) | يشير إلى ما إذا تمت الإشارة إلى هذا الاسم بواسطة صيغ أخرى.|
| [is_visible](/cells/ar/python-net/aspose.cells/name/is_visible) | يشير إلى ما إذا كان الاسم مرئيًا أم لا.|
| [sheet_index](/cells/ar/python-net/aspose.cells/name/sheet_index) | يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل.<br/> 0 = الاسم العام ، وإلا فهرسة إلى ورقة (مستند إلى واحد)|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/name/get_refers_to/#bool-bool) | احصل على مرجع هذا الاسم.|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/ar/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | احصل على مرجع هذا الاسم بناءً على الخلية المحددة.|
| [get_ranges()](/cells/ar/python-net/aspose.cells/name/get_ranges/#) |يحصل على جميع النطاقات المشار إليها بهذا الاسم.|
| [get_ranges(recalculate)](/cells/ar/python-net/aspose.cells/name/get_ranges/#bool) |يحصل على جميع النطاقات المشار إليها بهذا الاسم.|
| [get_range()](/cells/ar/python-net/aspose.cells/name/get_range/#) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق.|
| [get_range(recalculate)](/cells/ar/python-net/aspose.cells/name/get_range/#bool) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق|
| [get_range(sheet_index, row, column)](/cells/ar/python-net/aspose.cells/name/get_range/#int-int-int) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق.<br/> إذا لم يكن مرجع هذا الاسم مطلقًا ، فقد يختلف النطاق باختلاف الخلايا.|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) | قم بتعيين مرجع هذا الاسم.|
| [get_referred_areas(recalculate)](/cells/ar/python-net/aspose.cells/name/get_referred_areas/#bool) | يحصل على جميع المراجع المشار إليها بهذا الاسم.|



###  أمثلة

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [Name](/cells/ar/python-net/aspose.cells/name)
