---
title: page_count الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 180
url: /ar/python-net/aspose.cells/pptxsaveoptions/page_count/
is_root: false
---
##  page_count الملكية

الحصول على أو تحديد عدد الصفحات المراد حفظها.

###  ملاحظات

الافتراضي هو System.Int32.MaxValue مما يعني أنه سيتم عرض جميع الصفحات ..

###  مثال

يوضح المثال التالي كيفية عرض نطاق من الصفحات (3 و 4) في ملف Excel Microsoft إلى PDF.

```python
from aspose.cells import PdfSaveOptions, Workbook

# Open an Excel file
wb = Workbook("Book1.xlsx")
options = PdfSaveOptions()
# Print only Page 3 and Page 4 in the output PDF
# Starting page index (0-based index)
options.page_index = 3
# Number of pages to be printed
options.page_count = 2
# Save the PDF file
wb.save("output.pdf", options)

```
###  تعريف:
```python
@property
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PptxSaveOptions](/cells/ar/python-net/aspose.cells/pptxsaveoptions)
