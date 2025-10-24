##Sparkline.Column
Sparkline property. Gets the column index of the sparkline
## Sparkline.Column property
Gets the column index of the sparkline.
```csharp
public int Column { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklinePropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
// Create sparkline group
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 4;
ca.EndColumn = 4;
int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[groupIndex];
// Add sparkline at column 4 and demonstrate Column property
int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
Sparkline sparkline = group.Sparklines[sparklineIndex];
// Display column property (read-only)
Console.WriteLine("Sparkline Column: " + sparkline.Column);
// To change column position, we need to remove and re-add the sparkline
group.Sparklines.RemoveAt(sparklineIndex);
sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
sparkline = group.Sparklines[sparklineIndex];
Console.WriteLine("New Sparkline Column: " + sparkline.Column);
// Save workbook
workbook.Save("SparklineColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
