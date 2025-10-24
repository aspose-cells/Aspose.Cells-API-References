##MsoFormatPicture.LeftCropInch
MsoFormatPicture property. Represents the location of the left of the crop rectangle expressed in unit of inches
## MsoFormatPicture.LeftCropInch property
Represents the location of the left of the crop rectangle expressed, in unit of inches.
```csharp
public double LeftCropInch { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyLeftCropInchDemo
{
public static void Run()
{
// Create a workbook
var workbook = new Workbook();
var sheet = workbook.Worksheets[0];
// Load image data
byte[] imageData = File.ReadAllBytes("example.png");
// Add picture to worksheet
int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
var picture = sheet.Pictures[pictureIndex];
// Set and get LeftCropInch property
picture.FormatPicture.LeftCropInch = 0.5;
double leftCropValue = picture.FormatPicture.LeftCropInch;
Console.WriteLine($"Left crop value in inches: {leftCropValue}");
// Save the workbook
workbook.Save("LeftCropInchDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
