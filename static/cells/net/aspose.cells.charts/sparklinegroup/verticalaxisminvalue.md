##SparklineGroup.VerticalAxisMinValue
SparklineGroup property. Gets and sets the custom minimum value for the vertical axis
## SparklineGroup.VerticalAxisMinValue property
Gets and sets the custom minimum value for the vertical axis.
```csharp
public double VerticalAxisMinValue { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyVerticalAxisMinValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(5);
sheet.Cells["A2"].PutValue(2);
sheet.Cells["A3"].PutValue(1);
sheet.Cells["A4"].PutValue(3);
// Create sparkline group
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 3;
ca.StartColumn = 4;
ca.EndColumn = 4;
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Set vertical axis minimum value
group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
group.VerticalAxisMinValue = 0.0;
// Save the workbook
workbook.Save("SparklineVerticalAxisMinValueDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
