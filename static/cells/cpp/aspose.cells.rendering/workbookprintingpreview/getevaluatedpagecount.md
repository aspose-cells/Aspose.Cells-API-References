##Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method
'Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount method. Evaluate the total page count of this workbook in C++.'
## WorkbookPrintingPreview::GetEvaluatedPageCount method
Evaluate the total page count of this workbook.
```cpp
int32_t Aspose::Cells::Rendering::WorkbookPrintingPreview::GetEvaluatedPageCount()
```
## Examples
```cpp
Aspose::Cells::Startup();
//The following code shows the fastest way to get page count of a workbook.
Workbook workbook(u"Book1.xlsx");
WorkbookPrintingPreview workbookPrintingPreview(workbook, ImageOrPrintOptions());
//fastest way to get page count especailly when there are massive data in workbook.
int pageCount = workbookPrintingPreview.GetEvaluatedPageCount();
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [WorkbookPrintingPreview](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
