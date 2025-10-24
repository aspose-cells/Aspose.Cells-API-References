##MsoFormatPicture.RightCrop
MsoFormatPicture property. Represents the location of the right of the crop rectangle expressed expressed as a ratio of the images width
## MsoFormatPicture.RightCrop property
Represents the location of the right of the crop rectangle expressed, expressed as a ratio of the image's width.
```csharp
public double RightCrop { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class MsoFormatPicturePropertyRightCropDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[pictureIndex];
// Get the MsoFormatPicture of the picture
MsoFormatPicture msoFormatPicture = picture.FormatPicture;
// Display the current RightCrop value
Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);
// Set a new RightCrop value (0.2 means crop 20% from the right)
msoFormatPicture.RightCrop = 0.2;
Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);
// Save the workbook to see the effect
workbook.Save("RightCropDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
