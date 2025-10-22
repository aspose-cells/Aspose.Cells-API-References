##Cells.GetRowOriginalHeightPoint
Cells method. Gets original rows height in unit of point if the row is hidden
## Cells.GetRowOriginalHeightPoint method
Gets original row's height in unit of point if the row is hidden
```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
### Remarks
NOTE: This member is now obsolete. Instead, please use Cells.GetRowHeight(int,bool,CellsUnitType) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Store original height before modification
double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
// Modify row height
cells.SetRowHeight(0, 25.5);
try
{
// Get original height after modification
double originalHeight = cells.GetRowOriginalHeightPoint(0);
double currentHeight = cells.GetRowHeight(0);
Console.WriteLine($"Original row height: {originalHeight} points");
Console.WriteLine($"Current row height: {currentHeight} points");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
}
workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
