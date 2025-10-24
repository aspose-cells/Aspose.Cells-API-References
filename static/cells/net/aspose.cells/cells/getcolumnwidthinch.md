##Cells.GetColumnWidthInch
Cells method. Gets the width of the specified column in normal view in units of inches
## Cells.GetColumnWidthInch method
Gets the width of the specified column in normal view, in units of inches.
```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |
### Return Value
Width of column
Width of column in normal view.
### Remarks
NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetColumnWidthInchWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set column width in inches for demonstration
int columnIndex = 2;
cells.SetColumnWidthInch(columnIndex, 2.5);
try
{
// Call GetColumnWidthInch with Int32 parameter
double columnWidth = cells.GetColumnWidthInch(columnIndex);
// Display result
Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
