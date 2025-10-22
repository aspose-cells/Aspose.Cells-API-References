##PicFormatOption.Scale
PicFormatOption property. Gets or sets how many the picture stack and scale with
## PicFormatOption.Scale property
Gets or sets how many the picture stack and scale with.
```csharp
public double Scale { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO; // Added to resolve Stream-related issues
public class PicFormatOptionPropertyScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a 1x1 pixel BMP image byte array
byte[] bmpBytes = new byte[]
{
0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
0x00, 0x00, 0x00
};
// Add picture to the worksheet using MemoryStream
int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes)); // Fixed Stream conversion
Picture picture = worksheet.Pictures[pictureIndex];
// Configure picture position and size
picture.UpperLeftRow = 0;
picture.UpperLeftColumn = 0;
picture.LowerRightRow = 1;
picture.LowerRightColumn = 1;
// Get texture fill through FillFormat property
TextureFill textureFill = picture.Fill.TextureFill; // Fixed cast error
textureFill.PicFormatOption.Type = FillPictureType.Stack;
// Display and modify Scale property
PicFormatOption picFormat = textureFill.PicFormatOption;
Console.WriteLine("Current Scale value: " + picFormat.Scale);
picFormat.Scale = 0.5;
Console.WriteLine("Modified Scale value: " + picFormat.Scale);
// Expand cell dimensions to visualize effect
worksheet.Cells.SetRowHeight(0, 100);
worksheet.Cells.SetColumnWidth(0, 20);
// Save the workbook
workbook.Save("PropertyScaleDemo.xlsx");
}
}
}
```
### See Also
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
