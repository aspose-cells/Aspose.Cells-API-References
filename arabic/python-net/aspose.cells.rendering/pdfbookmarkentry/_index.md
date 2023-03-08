---
title: PdfBookmarkEntry الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 80
url: /ar/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  PdfBookmarkEntry الدرجة
PdfBookmarkEntry هو إدخال في المرجعية pdf.
إذا كانت خاصية Text للمثيل الحالي خالية أو "" ،
سيتم إخفاء المثيل الحالي وسيتم إدراج الأطفال في المستوى الحالي.



يكشف نوع PdfBookmarkEntry الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [PdfBookmarkEntry()](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | ينشئ مثيلاً جديدًا من PdfBookmarkEntry|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [text](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | عنوان إشارة مرجعية.|
| [destination](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | الخلية التي ترتبط بها الإشارة المرجعية.|
| [destination_name](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | يحصل أو يحدد اسم الوجهة.|
| [sub_entry](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | إدخال إشارة مرجعية فرعي.|
| [is_open](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) | عندما تكون هذه الخاصية صحيحة ، سيتم توسيع نقطة الإشارة المرجعية ، وإلا فسوف تنهار.|
| [is_collapse](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | عندما تكون هذه الخاصية صحيحة ، ستنهار نقطة الإشارة المرجعية ، وإلا فإنها ستتوسع.|



###  مثال

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering import PdfBookmarkEntry

workbook = Workbook()
workbook.worksheets.add()
workbook.worksheets.add()
cellInPage1 = workbook.worksheets[0].cells.get("A1")
cellInPage2 = workbook.worksheets[1].cells.get("A1")
cellInPage3 = workbook.worksheets[2].cells.get("A1")
cellInPage1.put_value("page1")
cellInPage2.put_value("page2")
cellInPage3.put_value("page3")
pbeRoot = PdfBookmarkEntry()
pbeRoot.text = "root"
pbeRoot.destination = cellInPage1
pbeRoot.sub_entry = []
pbeRoot.is_open = False
subPbe1 = PdfBookmarkEntry()
subPbe1.text = "section1"
subPbe1.destination = cellInPage2
subPbe2 = PdfBookmarkEntry()
subPbe2.text = "section2"
subPbe2.destination = cellInPage3
pbeRoot.sub_entry.append(subPbe1)
pbeRoot.sub_entry.append(subPbe2)
saveOptions = PdfSaveOptions()
saveOptions.bookmark = pbeRoot
workbook.save("output_bookmark.pdf", saveOptions)

```

###  أنظر أيضا
* وحدة [aspose.cells.rendering](..)
