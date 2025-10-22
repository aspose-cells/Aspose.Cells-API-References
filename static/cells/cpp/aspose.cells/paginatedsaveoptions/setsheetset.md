##Aspose::Cells::PaginatedSaveOptions::SetSheetSet method
'Aspose::Cells::PaginatedSaveOptions::SetSheetSet method. Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible in C++.'
## PaginatedSaveOptions::SetSheetSet method
Gets or sets the sheets to render. Default is all visible sheets in the workbook: Aspose.Cells.Rendering.SheetSet.Visible.
```cpp
void Aspose::Cells::PaginatedSaveOptions::SetSheetSet(const SheetSet &value)
```
## Examples
```cpp
Aspose::Cells::Startup();
//The following code only renders active sheet to pdf.
Workbook workbook(u"Book1.xlsx");
int activeSheetIndex = workbook.GetWorksheets().GetActiveSheetIndex();
PdfSaveOptions pdfSaveOptions;
//set active sheet index to sheet set.
SheetSet sheetSet(Vector<int>{ activeSheetIndex });
pdfSaveOptions.SetSheetSet(sheetSet);
workbook.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
