---
title: security_options propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 390
url: /fr/python-net/aspose.cells/pdfsaveoptions/security_options/
is_root: false
---
##  security_options propriété

Définissez ces options, lorsque la sécurité est nécessaire dans le résultat xls2pdf.

###  Exemple

Le code suivant définit l'autorisation d'impression haute résolution pour le pdf de sortie.

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
###  Définition:
```python
@property
def security_options(self):
    ...
@security_options.setter
def security_options(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [PdfSaveOptions](/cells/fr/python-net/aspose.cells/pdfsaveoptions)
* classe [PdfSecurityOptions](/cells/fr/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
