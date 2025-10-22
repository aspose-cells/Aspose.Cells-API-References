##TilePicOption.ScaleY
TilePicOption property. Gets or sets the Y scale for tiling picture
## TilePicOption.ScaleY property
Gets or sets the Y scale for tiling picture.
```csharp
public double ScaleY { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TilePicOptionPropertyScaleYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
Chart chart = worksheet.Charts[chartIndex];
// Set texture fill with image
chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
byte[] imageData = File.ReadAllBytes("example.png");
chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
// Configure tile options with ScaleY
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
// Save the workbook
workbook.Save("TilePicOptionScaleYDemo.xlsx");
}
}
}
```
### See Also
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
