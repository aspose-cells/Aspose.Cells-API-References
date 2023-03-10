---
title: PdfSecurityOptions Konstrukteur
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 10
url: /de/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/__init__/
is_root: false
---
##  PdfSecurityOptions() {#}
Der Konstruktor von PdfSecurityOptions



```python
def __init__(self):
    ...
```



###  Beispiel

Der folgende Code legt die Berechtigung zum Drucken in hoher Auflösung für das Ausgabe-PDF fest.

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



###  Siehe auch
* Modul [aspose.cells.rendering.pdfsecurity](../../)
* Klasse [PdfSecurityOptions](/cells/de/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
