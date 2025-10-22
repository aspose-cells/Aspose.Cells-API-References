##Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions constructor
'Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions constructor. The constructor of PdfSecurityOptions in C++.'
## PdfSecurityOptions::PdfSecurityOptions() constructor
The constructor of [PdfSecurityOptions](../).
```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions()
```
## Examples
```cpp
Aspose::Cells::Startup();
//The following code sets high resolution print permisson for the output pdf.
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
pdfSaveOptions.SetSecurityOptions(pdfSecurityOptions);
wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```
## See Also
* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
## PdfSecurityOptions::PdfSecurityOptions(PdfSecurityOptions_Impl*) constructor
Constructs from an implementation object.
```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions(PdfSecurityOptions_Impl *impl)
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
## PdfSecurityOptions::PdfSecurityOptions(const PdfSecurityOptions\&) constructor
Copy constructor.
```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions(const PdfSecurityOptions &src)
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PdfSecurityOptions](../)
* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
