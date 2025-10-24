##PdfSecurityOptions constructor
## \_\_init\_\_(self) {#}
The constructor of PdfSecurityOptions
```python
def __init__(self):
...
```
### Example
The following code sets high resolution print permisson for the output pdf.
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
### See Also
* module [`aspose.cells.rendering.pdfsecurity`](../../)
* class [`PdfSecurityOptions`](/cells/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
