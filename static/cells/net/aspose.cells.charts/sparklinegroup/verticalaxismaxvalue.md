##SparklineGroup.VerticalAxisMaxValue
SparklineGroup property. Gets and sets the custom maximum value for the vertical axis
## SparklineGroup.VerticalAxisMaxValue property
Gets and sets the custom maximum value for the vertical axis.
```csharp
public double VerticalAxisMaxValue { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyVerticalAxisMaxValueDemo
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
// Add sparkline
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Set vertical axis max value
group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Custom;
group.VerticalAxisMaxValue = 10.0;
// Save the workbook
workbook.Save("SparklineVerticalAxisMaxValueDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
