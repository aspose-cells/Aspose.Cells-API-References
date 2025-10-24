##FillFormat.Pattern
FillFormat property. Represents an areas display pattern
## FillFormat.Pattern property
Represents an area's display pattern.
```csharp
public FillPattern Pattern { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyPatternDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(50);
sheet.Cells["A2"].PutValue(100);
sheet.Cells["A3"].PutValue(150);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A1:A3", true);
// Access the first series and its first point
ChartPoint point = chart.NSeries[0].Points[0];
// Set fill pattern for the point's area
point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
// Save the workbook
workbook.Save("FillFormatPatternDemo.xlsx");
}
}
}
```
### See Also
* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
