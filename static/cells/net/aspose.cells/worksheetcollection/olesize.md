##WorksheetCollection.OleSize
WorksheetCollection property. Gets and Sets displayed size when Workbook file is used as an Ole object
## WorksheetCollection.OleSize property
Gets and Sets displayed size when Workbook file is used as an Ole object.
```csharp
public object OleSize { get; set; }
```
### Remarks
Null means no ole size setting.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyOleSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the OLE size for the worksheet collection
workbook.Worksheets.SetOleSize(0, 10, 0, 10);
// Access and display the OLE size properties
CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
Console.WriteLine("OLE Size Range:");
Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
// Save the workbook
workbook.Save("OleSizeDemo.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
