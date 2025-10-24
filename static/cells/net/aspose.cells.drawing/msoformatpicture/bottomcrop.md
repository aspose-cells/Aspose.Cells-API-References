##MsoFormatPicture.BottomCrop
MsoFormatPicture property. Represents the location of the bottom of the crop rectangle expressed expressed as a ratio of the images height
## MsoFormatPicture.BottomCrop property
Represents the location of the bottom of the crop rectangle expressed, expressed as a ratio of the image's height.
```csharp
public double BottomCrop { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class MsoFormatPicturePropertyBottomCropDemo
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
// Display the current BottomCrop value
Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);
// Set a new BottomCrop value (0.2 means crop 20% from the bottom)
msoFormatPicture.BottomCrop = 0.2;
Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);
// Set other crop values to demonstrate the effect
msoFormatPicture.TopCrop = 0.1;
msoFormatPicture.LeftCrop = 0.1;
msoFormatPicture.RightCrop = 0.1;
// Save the workbook to see the cropped picture
workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
