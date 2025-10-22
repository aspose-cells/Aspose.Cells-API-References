##PatternFill.Pattern
PatternFill property. Gets or sets the fill pattern type
## PatternFill.Pattern property
Gets or sets the fill pattern type
```csharp
public FillPattern Pattern { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PatternFillPropertyPatternDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
// Set chart data range
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Set fill pattern for first series
chart.NSeries[0].Area.FillFormat.FillType = FillType.Pattern;
chart.NSeries[0].Area.FillFormat.PatternFill.Pattern = FillPattern.WideDownwardDiagonal;
// Save the workbook
workbook.Save("PatternFillDemo.xlsx");
}
}
}
```
### See Also
* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
