##MsoFormatPicture.LeftCrop
MsoFormatPicture property. Represents the location of the left of the crop rectangle expressed expressed as a ratio of the images width
## MsoFormatPicture.LeftCrop property
Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width.
```csharp
public double LeftCrop { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyLeftCropDemo
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
// Set LeftCrop property
picture.FormatPicture.LeftCrop = 0.1;
Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);
// Get and set LeftCropInch property
double leftCropInch = picture.FormatPicture.LeftCropInch;
picture.FormatPicture.LeftCropInch = leftCropInch;
Console.WriteLine("LeftCropInch value: " + leftCropInch);
// Save the workbook
workbook.Save("LeftCropDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
