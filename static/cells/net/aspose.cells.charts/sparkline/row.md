##Sparkline.Row
Sparkline property. Gets the row index of the sparkline
## Sparkline.Row property
Gets the row index of the sparkline.
```csharp
public int Row { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklinePropertyRowDemo
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
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 0,
StartColumn = 4,
EndColumn = 4
};
int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[groupIndex];
// Add sparkline at row 0, column 4
int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
Sparkline sparkline = group.Sparklines[sparklineIndex];
// Display row position (read-only property)
Console.WriteLine("Sparkline row position: " + sparkline.Row);
// To change position, we need to remove and recreate the sparkline
group.Sparklines.RemoveAt(sparklineIndex);
sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
sparkline = group.Sparklines[sparklineIndex];
Console.WriteLine("New sparkline row position: " + sparkline.Row);
// Save workbook
workbook.Save("SparklineRowDemo.xlsx");
}
}
}
```
### See Also
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
