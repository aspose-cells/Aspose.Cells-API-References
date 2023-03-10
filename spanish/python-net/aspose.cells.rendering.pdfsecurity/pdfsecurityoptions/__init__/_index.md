---
title: PdfSecurityOptions constructor
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 10
url: /es/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/__init__/
is_root: false
---
##  PdfSecurityOptions() {#}
El constructor de PdfSecurityOptions



```python
def __init__(self):
    ...
```



###  Ejemplo

El siguiente código establece el permiso de impresión de alta resolución para el pdf de salida.

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



###  Ver también
* módulo [aspose.cells.rendering.pdfsecurity](../../)
* clase [PdfSecurityOptions](/cells/es/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
