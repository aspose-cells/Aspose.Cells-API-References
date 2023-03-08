---
title: page_index الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 320
url: /ar/python-net/aspose.cells/pdfsaveoptions/page_index/
is_root: false
---
##  page_index الملكية

الحصول على أو تحديد الفهرس الذي يستند إلى 0 للصفحة الأولى لحفظها.

###  ملاحظات

الافتراضي هو 0.

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
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [PdfSaveOptions](/cells/ar/python-net/aspose.cells/pdfsaveoptions)
