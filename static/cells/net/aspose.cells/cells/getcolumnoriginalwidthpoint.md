##Cells.GetColumnOriginalWidthPoint
Cells method. Gets original columns height in unit of point if the column is hidden
## Cells.GetColumnOriginalWidthPoint method
Gets original column's height in unit of point if the column is hidden
```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The row index. |
### Return Value
Width of column in normal view.
### Remarks
NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Prepare column index parameter
int columnIndex = 0;
try
{
// Get original column width in points
double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");
// Modify column width
cells.SetColumnWidth(columnIndex, 15);
Console.WriteLine("Set new column width to 15 points");
// Get original width again to demonstrate it remains unchanged
double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
Console.WriteLine($"Original width remains: {unchangedWidth} points");
// Get current width to show modification
double currentWidth = cells.GetColumnWidth(columnIndex);
Console.WriteLine($"Current column width: {currentWidth} points");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
}
// Save the modified workbook
workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
