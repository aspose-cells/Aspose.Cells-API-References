##Cells.IsRowHidden
Cells method. Checks whether a row at given index is hidden
## Cells.IsRowHidden method
Checks whether a row at given index is hidden.
```csharp
public bool IsRowHidden(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | row index |
### Return Value
true if the row is hidden
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodIsRowHiddenWithInt32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Sample data
cells[1, 0].PutValue("US");
cells[2, 0].PutValue("UK");
cells[3, 0].PutValue("India");
cells[4, 0].PutValue("UK");
cells[5, 0].PutValue("India");
cells[6, 0].PutValue("US");
// Apply filter
AutoFilter af = sheet.AutoFilter;
af.Range = "A1:A1";
af.Filter(0, "India");
af.Refresh();
// Check row visibility
Console.WriteLine("Row Visibility Check:");
for (int i = 1; i < 7; i++)
{
Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
