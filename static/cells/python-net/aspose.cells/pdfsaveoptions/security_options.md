##security_options property
## security_options property
Set this options, when security is need in xls2pdf result.
### Example
The following code sets hight resolution print permisson for the output pdf.
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
### Definition:
```python
@property
def security_options(self):
...
@security_options.setter
def security_options(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`PdfSaveOptions`](/cells/python-net/aspose.cells/pdfsaveoptions)
* class [`PdfSecurityOptions`](/cells/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
