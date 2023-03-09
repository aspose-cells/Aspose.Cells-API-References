---
title: ExternalLink الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 560
url: /ar/python-net/aspose.cells/externallink/
is_root: false
---
##  ExternalLink الدرجة
يمثل ارتباطًا خارجيًا في مصنف.



يكشف نوع ExternalLink الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [type](/cells/ar/python-net/aspose.cells/externallink/type) | يحصل على نوع الارتباط الخارجي.|
| [original_data_source](/cells/ar/python-net/aspose.cells/externallink/original_data_source) | يمثل مصدر البيانات المخزنة للارتباط الخارجي.|
| [data_source](/cells/ar/python-net/aspose.cells/externallink/data_source) | يمثل مصدر بيانات الارتباط الخارجي.|
| [is_referred](/cells/ar/python-net/aspose.cells/externallink/is_referred) | يشير إلى ما إذا كان الآخرون قد أشاروا إلى هذا الارتباط الخارجي.|
| [is_visible](/cells/ar/python-net/aspose.cells/externallink/is_visible) | يشير إلى ما إذا كان هذا الارتباط الخارجي مرئيًا في MS Excel.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add_external_name(text, refer_to)](/cells/ar/python-net/aspose.cells/externallink/add_external_name/#str-str) | يضيف اسمًا خارجيًا.|



###  أمثلة

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
