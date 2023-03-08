---
title: printing_page_type الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 210
url: /ar/python-net/aspose.cells/pptxsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type الملكية

يشير إلى الصفحات التي لن تتم طباعتها.

###  ملاحظات

إذا كان المحتوى في الورقة متناثرًا ، فستكون هناك بعض الصفحات فارغة تمامًا في ملف pdf الناتج.
إذا كنت لا تريد هذه الصفحات الفارغة ، يمكنك استخدام هذا الخيار لحذفها.

###  مثال

يحذف الكود التالي الصفحات أو الصفحات الفارغة التي تحتوي فقط على بعض محتوى النمط مثل خلفية الخلية والحدود.

```python
from aspose.cells import PdfSaveOptions, PrintingPageType, Workbook

wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# ignore blank pages
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_BLANK
wb.save("output_ignore_blank_page.pdf", pdfSaveOptions)
# ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_STYLE
wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions)

```
###  تعريف:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PptxSaveOptions](/cells/ar/python-net/aspose.cells/pptxsaveoptions)
* فئة [PrintingPageType](/cells/ar/python-net/aspose.cells/printingpagetype)
