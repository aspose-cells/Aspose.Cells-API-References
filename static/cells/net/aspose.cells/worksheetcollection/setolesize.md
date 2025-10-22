##WorksheetCollection.SetOleSize
WorksheetCollection method. Sets displayed size when Workbook file is used as an Ole object
## WorksheetCollection.SetOleSize method
Sets displayed size when Workbook file is used as an Ole object.
```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |
### Remarks
This method is generally used to adjust display size in ppt file or doc file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set OLE size for the worksheets
workbook.Worksheets.SetOleSize(0, 10, 0, 10);
// Save the workbook
workbook.Save("output.xlsx");
// Verify the OLE size
Workbook loadedWorkbook = new Workbook("output.xlsx");
CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}",
oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
