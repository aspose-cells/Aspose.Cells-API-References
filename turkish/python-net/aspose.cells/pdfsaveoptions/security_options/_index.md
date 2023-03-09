---
title: security_options mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 390
url: /tr/python-net/aspose.cells/pdfsaveoptions/security_options/
is_root: false
---
##  security_options mülk

xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın.

###  örnekler

Aşağıdaki kod, çıktı pdf için yüksek çözünürlüklü yazdırma iznini ayarlar.

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering.pdfsecurity import PdfSecurityOptions

wb = Workbook()
wb.worksheets[0].cells.get("A1").value = "Aspose"
pdfSaveOptions = PdfSaveOptions()
pdfSecurityOptions = PdfSecurityOptions()
# set owner password
pdfSecurityOptions.owner_password = "YourOwnerPassword"
# set user password
pdfSecurityOptions.user_password = "YourUserPassword"
# set print permisson
pdfSecurityOptions.print_permission = True
# set high resolution for print
pdfSecurityOptions.full_quality_print_permission = True
pdfSaveOptions.security_options = pdfSecurityOptions
wb.save("output.pdf", pdfSaveOptions)

```
###  Tanım:
```python
@property
def security_options(self):
    ...
@security_options.setter
def security_options(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PdfSaveOptions](/cells/tr/python-net/aspose.cells/pdfsaveoptions)
* sınıf [PdfSecurityOptions](/cells/tr/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
