##Cells.GetRowHeightInch
Cells method. Gets the height of a specified row in unit of inches
## Cells.GetRowHeightInch method
Gets the height of a specified row in unit of inches.
```csharp
public double GetRowHeightInch(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
### Return Value
Height of row
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetRowHeightInchWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set row height in inches for row 5
cells.SetRowHeightInch(5, 1.5);
// Get row height in inches for row 5
double rowHeight = cells.GetRowHeightInch(5);
// Output the result
Console.WriteLine("Row height in inches: " + rowHeight);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
