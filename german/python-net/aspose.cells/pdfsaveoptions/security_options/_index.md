---
title: security_options Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 390
url: /de/python-net/aspose.cells/pdfsaveoptions/security_options/
is_root: false
---
##  security_options Eigentum

Stellen Sie diese Optionen ein, wenn Sicherheit im xls2pdf-Ergebnis benötigt wird.

###  Beispiele

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
###  Definition:
```python
@property
def security_options(self):
    ...
@security_options.setter
def security_options(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PdfSaveOptions](/cells/de/python-net/aspose.cells/pdfsaveoptions)
* Klasse [PdfSecurityOptions](/cells/de/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
