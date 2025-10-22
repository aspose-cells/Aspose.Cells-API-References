##Cells.GetViewRowHeight
Cells method. Gets the height of a specified row
## Cells.GetViewRowHeight method
Gets the height of a specified row.
```csharp
public double GetViewRowHeight(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
### Return Value
Height of row.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetViewRowHeightWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set row height for row 3 (in points)
worksheet.Cells.SetRowHeight(3, 15);
// Get the view row height for row 3
double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
// Output the result
Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
