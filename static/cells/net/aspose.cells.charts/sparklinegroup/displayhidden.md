##SparklineGroup.DisplayHidden
SparklineGroup property. Indicates whether to show data in hidden rows and columns
## SparklineGroup.DisplayHidden property
Indicates whether to show data in hidden rows and columns.
```csharp
public bool DisplayHidden { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyDisplayHiddenDemo
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
// Define sparkline location
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add sparkline group
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Add sparkline to the group
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Configure sparkline appearance
CellsColor seriesColor = workbook.CreateCellsColor();
seriesColor.Color = Color.Blue;
group.SeriesColor = seriesColor;
// Demonstrate DisplayHidden property
group.DisplayHidden = true; // Show sparklines for hidden data
// Save the workbook
workbook.Save("SparklineDisplayHiddenDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
