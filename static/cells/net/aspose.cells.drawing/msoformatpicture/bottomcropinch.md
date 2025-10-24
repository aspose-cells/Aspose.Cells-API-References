##MsoFormatPicture.BottomCropInch
MsoFormatPicture property. Represents the location of the bottom of the crop rectangle expressed in unit of inches
## MsoFormatPicture.BottomCropInch property
Represents the location of the bottom of the crop rectangle expressed, in unit of inches.
```csharp
public double BottomCropInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyBottomCropInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a picture to the worksheet (using a placeholder path)
int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
Picture picture = sheet.Pictures[pictureIndex];
// Access the MsoFormatPicture object
MsoFormatPicture formatPicture = picture.FormatPicture;
// Set the BottomCropInch property and demonstrate its usage
formatPicture.BottomCropInch = 0.3;
formatPicture.TopCropInch = 0.2;
// Save the workbook
workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
