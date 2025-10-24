##FillFormat.PresetColor
FillFormat property. Returns the gradient preset color for the specified fill
## FillFormat.PresetColor property
Returns the gradient preset color for the specified fill.
```csharp
public GradientPresetType PresetColor { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyPresetColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Access the fill format of the chart area
FillFormat fillFormat = chart.ChartArea.Area.FillFormat;
// Set a gradient preset color
fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);
// Display and verify the preset color
Console.WriteLine("Preset Color: " + fillFormat.PresetColor);
// Save the workbook
workbook.Save("FillFormatPresetColorDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
