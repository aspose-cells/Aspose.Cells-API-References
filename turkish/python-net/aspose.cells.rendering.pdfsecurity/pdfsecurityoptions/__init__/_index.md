---
title: PdfSecurityOptions yapıcı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/__init__/
is_root: false
---
##  PdfSecurityOptions() {#}
PdfSecurityOptions'in kurucusu



```python
def __init__(self):
    ...
```



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



###  Ayrıca bakınız
* modül [aspose.cells.rendering.pdfsecurity](../../)
* sınıf [PdfSecurityOptions](/cells/tr/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
