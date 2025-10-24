##Line.WeightPx
Line property. Gets or sets the weight of the line in unit of pixels
## Line.WeightPx property
Gets or sets the weight of the line in unit of pixels.
```csharp
public double WeightPx { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyWeightPxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Add sample data
cells["A1"].PutValue(10);
cells["A2"].PutValue(20);
cells["A3"].PutValue(30);
cells["B1"].PutValue(15);
cells["B2"].PutValue(25);
cells["B3"].PutValue(35);
// Add a line chart
int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure line properties with WeightPx
Aspose.Cells.Charts.Series series = chart.NSeries[0];
series.Border.WeightPx = 5.0; // Set line weight in pixels
series.Border.Color = System.Drawing.Color.Blue;
// Save the workbook
workbook.Save("LineWeightPxDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
