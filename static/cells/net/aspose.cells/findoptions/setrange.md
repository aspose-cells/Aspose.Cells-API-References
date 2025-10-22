##FindOptions.SetRange
FindOptions method. Sets the searched range
## FindOptions.SetRange method
Sets the searched range.
```csharp
public void SetRange(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the searched range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsMethodSetRangeWithCellAreaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("abc");
worksheet.Cells["B2"].PutValue("def");
worksheet.Cells["C3"].PutValue("abc");
// Create FindOptions and set search range
FindOptions rangeOptions = new FindOptions();
CellArea cellarea = new CellArea();
cellarea.StartRow = 1;
cellarea.StartColumn = 1;
cellarea.EndRow = 3;
cellarea.EndColumn = 3;
rangeOptions.SetRange(cellarea);
// Search within the specified range
rangeOptions.SearchBackward = false;
Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
