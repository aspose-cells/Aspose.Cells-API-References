---
title: QueryTable الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1230
url: /ar/python-net/aspose.cells/querytable/
is_root: false
---
##  QueryTable الدرجة
يمثل QueryTable معلومات.



يكشف نوع QueryTable الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [connection_id](/cells/ar/python-net/aspose.cells/querytable/connection_id) |يحصل على معرف الاتصال لجدول الاستعلام.|
| [external_connection](/cells/ar/python-net/aspose.cells/querytable/external_connection) | يحصل على اتصال خارجي.|
| [name](/cells/ar/python-net/aspose.cells/querytable/name) | يحصل على اسم الاستعلام.|
| [result_range](/cells/ar/python-net/aspose.cells/querytable/result_range) | يحصل على مدى النتيجة.|
| [preserve_formatting](/cells/ar/python-net/aspose.cells/querytable/preserve_formatting) | إرجاع أو تعيين PreserveFormatting للكائن.|
| [adjust_column_width](/cells/ar/python-net/aspose.cells/querytable/adjust_column_width) | إرجاع أو تعيين AdjustColumnWidth للكائن.|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Getting the first query table in the worksheet
qt = worksheet.query_tables[0]
# Getting display address of the query table.
address = qt.result_range.address

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
