##Aspose::Cells::Rendering::SheetRender::GetPageScale method
'Aspose::Cells::Rendering::SheetRender::GetPageScale method. Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall in C++.'
## SheetRender::GetPageScale method
Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall.
```cpp
double Aspose::Cells::Rendering::SheetRender::GetPageScale()
```
## Examples
```cpp
Aspose::Cells::Startup();
Workbook wb(u"Book1.xlsx");
SheetRender sheetRender(wb.GetWorksheets().Get(0), ImageOrPrintOptions());
//Gets calculated page scale of the sheet.
double pageScale = sheetRender.GetPageScale();
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
