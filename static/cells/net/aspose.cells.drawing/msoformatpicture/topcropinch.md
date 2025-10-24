##MsoFormatPicture.TopCropInch
MsoFormatPicture property. Represents the location of the top of the crop rectangle expressed in unit of inches
## MsoFormatPicture.TopCropInch property
Represents the location of the top of the crop rectangle expressed, in unit of inches.
```csharp
public double TopCropInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyTopCropInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a picture (replace with actual image path)
int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];
// Access and modify TopCropInch property
Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
format.TopCropInch = 0.3; // Crop 0.3 inches from top
format.BottomCropInch = 0.2; // Additional crop properties for context
// Save the result
workbook.Save("TopCropInchDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
