##TilePicOption.ScaleX
TilePicOption property. Gets or sets the X scale for tiling picture
## TilePicOption.ScaleX property
Gets or sets the X scale for tiling picture.
```csharp
public double ScaleX { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TilePicOptionPropertyScaleXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and create a chart
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Set texture fill with image
string imagePath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "texture.png");
byte[] imageData = File.ReadAllBytes(imagePath);
chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
// Demonstrate ScaleX property
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50; // 50% horizontal scaling
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 75; // 75% vertical scaling
// Save the workbook
workbook.Save(Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ScaleXDemo.xlsx"));
}
}
}
```
### See Also
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
