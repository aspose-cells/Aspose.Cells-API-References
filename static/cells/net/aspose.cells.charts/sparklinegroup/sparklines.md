##SparklineGroup.Sparklines
SparklineGroup property. Gets the collection of Sparkline object
## SparklineGroup.Sparklines property
Gets the collection of [`Sparkline`](../../sparkline/) object.
```csharp
public SparklineCollection Sparklines { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertySparklinesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["C1"].PutValue(1);
worksheet.Cells["D1"].PutValue(3);
// Create sparkline group
CellArea location = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 4, EndColumn = 4 };
int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
SparklineGroup group = worksheet.SparklineGroups[groupIndex];
// Add sparkline using Sparklines property
group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);
// Customize sparkline appearance
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Blue;
group.SeriesColor = color;
// Save the workbook
workbook.Save("SparklineDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
