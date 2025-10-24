##PivotField.Position
PivotField property. Represents the index of PivotField in the region
## PivotField.Position property
Represents the index of [`PivotField`](../) in the region.
```csharp
public int Position { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyPositionDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook wb = new Workbook("NET46429_a.xlsx");
// Access first worksheet and its pivot table
Worksheet ws = wb.Worksheets[0];
PivotTable pt = ws.PivotTables[0];
// Demonstrate Position property usage
int position = pt.PageFields[0].Position;
Console.WriteLine("Position of first page field: " + position);
// Use position to show report filter pages
pt.ShowReportFilterPageByIndex(position);
// Save the workbook
wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
