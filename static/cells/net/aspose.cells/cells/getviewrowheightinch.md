##Cells.GetViewRowHeightInch
Cells method. Gets the height of a specified row in unit of inches
## Cells.GetViewRowHeightInch method
Gets the height of a specified row in unit of inches.
```csharp
public double GetViewRowHeightInch(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
### Return Value
Height of row
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetViewRowHeightInchWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set custom row height for row 2 in inches
worksheet.Cells.SetRowHeightInch(2, 1.5);
try
{
// Call GetViewRowHeightInch with row index parameter
double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
// Display result and verify height matches set value
Console.WriteLine($"View row height of row 2: {rowHeight} inches");
// Demonstrate effect by adding sample content
worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
worksheet.Cells.SetColumnWidthInch(0, 15);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
}
// Save the modified workbook
workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
