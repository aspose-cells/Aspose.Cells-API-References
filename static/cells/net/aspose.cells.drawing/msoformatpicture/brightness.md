##MsoFormatPicture.Brightness
MsoFormatPicture property. Represents the brightness modification for the picture in unit of percentage
## MsoFormatPicture.Brightness property
Represents the brightness modification for the picture in unit of percentage.
```csharp
public double Brightness { get; set; }
```
### Remarks
It is between -100% and 100%. It works same as Excel 2007 or above version.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyBrightnessDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];
// Set and get brightness
picture.FormatPicture.Brightness = 30;
Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);
// Modify brightness
picture.FormatPicture.Brightness = 70;
Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
