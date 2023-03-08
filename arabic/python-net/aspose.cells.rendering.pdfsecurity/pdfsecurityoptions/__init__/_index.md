---
title: PdfSecurityOptions المنشئ
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 10
url: /ar/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/__init__/
is_root: false
---
##  PdfSecurityOptions() {#}
منشئ PdfSecurityOptions



```python
def __init__(self):
    ...
```



###  مثال

يحدد الكود التالي إذن طباعة عالي الدقة لملف pdf.

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



###  أنظر أيضا
* وحدة [aspose.cells.rendering.pdfsecurity](../../)
* فئة [PdfSecurityOptions](/cells/ar/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
