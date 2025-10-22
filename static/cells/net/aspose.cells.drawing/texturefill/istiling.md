##TextureFill.IsTiling
TextureFill property. Indicates whether tile picture as texture
## TextureFill.IsTiling property
Indicates whether tile picture as texture.
```csharp
public bool IsTiling { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextureFillPropertyIsTilingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("A1:B3", true);
// Set texture fill for plot area
chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
// Set IsTiling property
chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
// Verify and output the IsTiling value
Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
// Save the workbook
workbook.Save("TextureFillIsTilingDemo.xlsx");
}
}
}
```
### See Also
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
