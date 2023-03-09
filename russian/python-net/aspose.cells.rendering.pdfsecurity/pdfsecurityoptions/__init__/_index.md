---
title: PdfSecurityOptions конструктор
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/__init__/
is_root: false
---
##  PdfSecurityOptions() {#}
Конструктор PdfSecurityOptions



```python
def __init__(self):
    ...
```



###  Примеры

Следующий код устанавливает разрешение на печать с высоким разрешением для выходного PDF-файла.

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



###  Смотрите также
* модуль [aspose.cells.rendering.pdfsecurity](../../)
* класс [PdfSecurityOptions](/cells/ru/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
