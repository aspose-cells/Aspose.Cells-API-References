##Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method
'Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this worksheet in C++.'
## SheetPrintingPreview::GetEvaluatedPageCount method
Evaluate the total page count of this worksheet.
```cpp
int32_t Aspose::Cells::Rendering::SheetPrintingPreview::GetEvaluatedPageCount()
```
## Examples
```cpp
Aspose::Cells::Startup();
//The following code shows the fastest way to get page count of a worksheet.
Workbook workbook(u"Book1.xlsx");
SheetPrintingPreview sheetPrintingPreview(workbook.GetWorksheets().Get(0), ImageOrPrintOptions());
//fastest way to get page count especailly when there are massive data in worksheet.
int pageCount = sheetPrintingPreview.GetEvaluatedPageCount();
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
