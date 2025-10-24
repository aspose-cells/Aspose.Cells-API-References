##Enum SparklineType
Aspose.Cells.Charts.SparklineType enum. Represents the sparkline types
## SparklineType enumeration
Represents the sparkline types.
```csharp
public enum SparklineType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Line | `0` | Line sparkline. |
| Column | `1` | Column sparkline. |
| Stacked | `2` | Win/Loss sparkline. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class SparklineTypeDemo
{
public static void SparklineTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["C1"].PutValue(1);
worksheet.Cells["D1"].PutValue(3);
// Define the CellArea for the sparkline
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add a sparkline group to the worksheet
int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = worksheet.SparklineGroups[idx];
// Add sparklines to the group
group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);
// Customize the sparkline group
CellsColor clr = workbook.CreateCellsColor();
clr.Color = Color.Orange;
group.SeriesColor = clr;
// Set the high points to be colored green and the low points to be colored red
group.ShowHighPoint = true;
group.ShowLowPoint = true;
group.HighPointColor.Color = Color.Green;
group.LowPointColor.Color = Color.Red;
// Set line weight
group.LineWeight = 1.0;
// Save the workbook
workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
