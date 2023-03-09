---
title: security_options недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 390
url: /ru/python-net/aspose.cells/pdfsaveoptions/security_options/
is_root: false
---
##  security_options недвижимость

Установите эти параметры, если требуется безопасность в результате xls2pdf.

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
###  Определение:
```python
@property
def security_options(self):
    ...
@security_options.setter
def security_options(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PdfSaveOptions](/cells/ru/python-net/aspose.cells/pdfsaveoptions)
* класс [PdfSecurityOptions](/cells/ru/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
