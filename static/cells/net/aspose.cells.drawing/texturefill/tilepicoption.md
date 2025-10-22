##TextureFill.TilePicOption
TextureFill property. Gets or sets tile picture option
## TextureFill.TilePicOption property
Gets or sets tile picture option.
```csharp
public TilePicOption TilePicOption { get; set; }
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
public class TextureFillPropertyTilePicOptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set texture fill with image
chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
byte[] imageData = File.ReadAllBytes("texture.png");
chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
// Configure tile options
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetX = 10;
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetY = 10;
// Save the workbook
workbook.Save("TextureFillDemo.xlsx");
}
}
}
```
### See Also
* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
