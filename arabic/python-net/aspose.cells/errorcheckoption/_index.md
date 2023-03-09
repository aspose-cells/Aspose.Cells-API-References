---
title: ErrorCheckOption الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 520
url: /ar/python-net/aspose.cells/errorcheckoption/
is_root: false
---
##  ErrorCheckOption الدرجة
تم تطبيق إعداد التحقق من الخطأ على نطاقات معينة.



يكشف نوع ErrorCheckOption الأعضاء التالية:

###  طُرق
| طريقة| وصف|
| :- | :- |
| [is_error_check(error_check_type)](/cells/ar/python-net/aspose.cells/errorcheckoption/is_error_check/#ErrorCheckType) | للتحقق مما إذا كان سيتم التحقق من نوع الخطأ المحدد.|
| [set_error_check(error_check_type, is_check)](/cells/ar/python-net/aspose.cells/errorcheckoption/set_error_check/#ErrorCheckType-bool) | يحدد ما إذا كان سيتم التحقق من نوع الخطأ المحدد.|
| [get_count_of_range()](/cells/ar/python-net/aspose.cells/errorcheckoption/get_count_of_range/#) | الحصول على عدد النطاقات التي تأثرت بهذا الإعداد.|
| [add_range(ca)](/cells/ar/python-net/aspose.cells/errorcheckoption/add_range/#CellArea) | يضيف نطاقًا واحدًا متأثرًا بهذا الإعداد.|
| [get_range(index)](/cells/ar/python-net/aspose.cells/errorcheckoption/get_range/#int) | يحصل على النطاق المتأثر لهذا الإعداد بفهرس معين.|
| [remove_range(index)](/cells/ar/python-net/aspose.cells/errorcheckoption/remove_range/#int) | يزيل نطاق واحد بفهرس معين.|



###  أمثلة

```python
from aspose.cells import CellArea, ErrorCheckType, Workbook

workbook = Workbook()
opts = workbook.worksheets[0].error_check_options
optionIdx = opts.add()
opt = opts[optionIdx]
opt.set_error_check(ErrorCheckType.INCONSIST_FORMULA, False)
opt.set_error_check(ErrorCheckType.INCONSIST_RANGE, False)
opt.set_error_check(ErrorCheckType.TEXT_DATE, False)
opt.set_error_check(ErrorCheckType.TEXT_NUMBER, False)
opt.set_error_check(ErrorCheckType.VALIDATION, False)
opt.add_range(CellArea.create_cell_area("A1", "B10"))
workbook.save(r"Book1.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
