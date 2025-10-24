##MsoFormatPicture.RightCropInch
MsoFormatPicture property. Represents the location of the right of the crop rectangle expressed in unit of inches
## MsoFormatPicture.RightCropInch property
Represents the location of the right of the crop rectangle expressed, in unit of inches.
```csharp
public double RightCropInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyRightCropInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a picture (replace with actual image path)
int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];
// Access and set RightCropInch property
Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
format.RightCropInch = 0.3; // Crop 0.3 inches from right
// Save the workbook
workbook.Save("RightCropInchDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
