---
title: ExternalLinkCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 570
url: /ar/python-net/aspose.cells/externallinkcollection/
is_root: false
---
##  ExternalLinkCollection الدرجة
يمثل مجموعة الارتباطات الخارجية في مصنف.



يكشف نوع ExternalLinkCollection الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [count](/cells/ar/python-net/aspose.cells/externallinkcollection/count) | الحصول على عدد العناصر الموجودة بالفعل في المجموعة.|



الحصول على عنصر [ExternalLink](/cells/ar/python-net/aspose.cells/externallink) بالفهرس المحدد.
###  مفهرس
| اسم| وصف|
| :- | :- |
| [index] | الفهرس الصفري للعنصر.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(file_name, sheet_names)](/cells/ar/python-net/aspose.cells/externallinkcollection/add/#str-list) | يضيف ارتباط خارجي.|
| [add(directory_type, file_name, sheet_names)](/cells/ar/python-net/aspose.cells/externallinkcollection/add/#DirectoryType-str-list) | أضف ارتباطًا خارجيًا.|
| [clear()](/cells/ar/python-net/aspose.cells/externallinkcollection/clear/#) | يزيل كل الروابط الخارجية.|
| [clear(update_references_as_local)](/cells/ar/python-net/aspose.cells/externallinkcollection/clear/#bool) | يزيل كل الروابط الخارجية.|
| [remove_at(index)](/cells/ar/python-net/aspose.cells/externallinkcollection/remove_at/#int) | يزيل الارتباط الخارجي المحدد من المصنف.|
| [remove_at(index, update_references_as_local)](/cells/ar/python-net/aspose.cells/externallinkcollection/remove_at/#int-bool) | يزيل الارتباط الخارجي المحدد من المصنف.|



###  مثال

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Change external link data source
workbook.worksheets.external_links[0].data_source = "d:\\link.xls"

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [ExternalLink](/cells/ar/python-net/aspose.cells/externallink)
