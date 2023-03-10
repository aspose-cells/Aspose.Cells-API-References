---
title: page_index mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 190
url: /tr/python-net/aspose.cells/xpssaveoptions/page_index/
is_root: false
---
##  page_index mülk

Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar.

###  Notlar

Varsayılan 0'dır.

###  Örnek

Aşağıdaki örnek, bir Microsoft Excel dosyasındaki sayfa aralığının (3 ve 4) PDF'e nasıl dönüştürüleceğini gösterir.

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
###  Tanım:
```python
@property
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [XpsSaveOptions](/cells/tr/python-net/aspose.cells/xpssaveoptions)
