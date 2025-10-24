##FillFormat.GradientStyle
FillFormat property. Returns the gradient style for the specified fill
## FillFormat.GradientStyle property
Returns the gradient style for the specified fill.
```csharp
public GradientStyleType GradientStyle { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyGradientStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a chart and get its chart area
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
Chart chart = sheet.Charts[chartIndex];
ChartArea chartArea = chart.ChartArea;
// Set gradient fill style
chartArea.Area.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Vertical, 2);
// Demonstrate GradientStyle property usage
Console.WriteLine("Gradient Style: " + chartArea.Area.FillFormat.GradientStyle);
// Save the workbook
workbook.Save("FillFormatPropertyGradientStyleDemo_out.xlsx");
}
}
}
```
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
