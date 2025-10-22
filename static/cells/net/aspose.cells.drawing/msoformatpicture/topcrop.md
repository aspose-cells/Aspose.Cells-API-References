##MsoFormatPicture.TopCrop
MsoFormatPicture property. Represents the location of the top of the crop rectangle expressed expressed as a ratio of the images height
## MsoFormatPicture.TopCrop property
Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height.
```csharp
public double TopCrop { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyTopCropDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
// Set TopCrop property
picture.FormatPicture.TopCrop = -6;
// Output the TopCrop value
Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
// Save the workbook
workbook.Save("TopCropDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
