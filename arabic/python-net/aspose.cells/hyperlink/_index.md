---
title: Hyperlink الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 790
url: /ar/python-net/aspose.cells/hyperlink/
is_root: false
---
##  Hyperlink الدرجة
لتغليف الكائن الذي يمثل ارتباطًا تشعبيًا.



يكشف نوع Hyperlink الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [address](/cells/ar/python-net/aspose.cells/hyperlink/address) | يمثل عنوان الارتباط التشعبي.|
| [text_to_display](/cells/ar/python-net/aspose.cells/hyperlink/text_to_display) | يمثل النص الذي سيتم عرضه للارتباط التشعبي المحدد. القيمة الافتراضية هي عنوان الارتباط التشعبي.|
| [area](/cells/ar/python-net/aspose.cells/hyperlink/area) | يحصل على نطاق الارتباط التشعبي.|
| [screen_tip](/cells/ar/python-net/aspose.cells/hyperlink/screen_tip) | إرجاع أو تعيين نص تلميح الشاشة للارتباط التشعبي المحدد.|
| [link_type](/cells/ar/python-net/aspose.cells/hyperlink/link_type) | يحصل على نوع الارتباط.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [delete()](/cells/ar/python-net/aspose.cells/hyperlink/delete/#) | يحذف هذا الارتباط التشعبي|



###  مثال

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Adding a hyperlink to a URL at "A1" cell
index = worksheet.hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Getting a Hyperlink by index.
hyperlink = worksheet.hyperlinks[index]
# Setting display text of this hyperlink.
hyperlink.text_to_display = "Aspose"
# Saving the Excel file
workbook.save("book1.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
