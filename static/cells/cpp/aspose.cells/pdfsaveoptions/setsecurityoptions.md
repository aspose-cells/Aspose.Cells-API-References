##Aspose::Cells::PdfSaveOptions::SetSecurityOptions method
'Aspose::Cells::PdfSaveOptions::SetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
## PdfSaveOptions::SetSecurityOptions method
Set this options, when security is need in xls2pdf result.
```cpp
void Aspose::Cells::PdfSaveOptions::SetSecurityOptions(const PdfSecurityOptions &value)
```
## Examples
```cpp
Aspose::Cells::Startup();
//The following code sets hight resolution print permisson for the output pdf.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");
PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;
//set owner password
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");
//set user password
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");
//set print permisson
pdfSecurityOptions.SetPrintPermission(true);
//set high resolution for print
pdfSecurityOptions.SetFullQualityPrintPermission(true);
if (pdfSaveOptions.GetSecurityOptions().IsNull())
{
pdfSaveOptions.SetSecurityOptions(pdfSecurityOptions);
}
wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
