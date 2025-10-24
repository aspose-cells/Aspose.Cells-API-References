##SparklineGroup.HorizontalAxisDateRange
SparklineGroup property. Represents the range that contains the date values for the sparkline data
## SparklineGroup.HorizontalAxisDateRange property
Represents the range that contains the date values for the sparkline data.
```csharp
public string HorizontalAxisDateRange { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyHorizontalAxisDateRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add date and value data for the sparkline
sheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
sheet.Cells["B1"].PutValue(new DateTime(2023, 2, 1));
sheet.Cells["C1"].PutValue(new DateTime(2023, 3, 1));
sheet.Cells["D1"].PutValue(new DateTime(2023, 4, 1));
sheet.Cells["A2"].PutValue(5);
sheet.Cells["B2"].PutValue(2);
sheet.Cells["C2"].PutValue(1);
sheet.Cells["D2"].PutValue(3);
// Define the CellArea where sparkline will be placed
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 1,
EndRow = 1
};
// Add a sparkline group with date axis
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A2:D2", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Set the date range for horizontal axis
group.HorizontalAxisDateRange = "A1:D1";
group.ShowHorizontalAxis = true;
// Save the workbook
workbook.Save("SparklineWithDateAxis.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
