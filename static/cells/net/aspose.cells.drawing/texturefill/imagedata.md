##TextureFill.ImageData
TextureFill property. Gets and sets the image data of the fill
## TextureFill.ImageData property
Gets and sets the image data of the fill.
```csharp
public byte[] ImageData { get; set; }
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
public class TextureFillPropertyImageDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
Chart chart = worksheet.Charts[chartIndex];
// Set texture fill type
chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
// Load image data
byte[] imageData = File.ReadAllBytes("texture.png");
// Set image data for texture fill
chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
// Save the workbook
workbook.Save("TextureFillDemo.xlsx");
}
}
}
```
### See Also
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
