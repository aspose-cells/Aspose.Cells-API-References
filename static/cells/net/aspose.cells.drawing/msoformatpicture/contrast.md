##MsoFormatPicture.Contrast
MsoFormatPicture property. Represents the contrast modification for the picture.in unit of percentage
## MsoFormatPicture.Contrast property
Represents the contrast modification for the picture.in unit of percentage.
```csharp
public double Contrast { get; set; }
```
### Remarks
It is between -100% and 100%. It works same as Excel 2007 or above version.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyContrastDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
var picture = worksheet.Pictures[pictureIndex];
// Set and get contrast value
picture.FormatPicture.Contrast = 50;
Console.WriteLine("Current contrast: " + picture.FormatPicture.Contrast);
// Modify contrast
picture.FormatPicture.Contrast = 75;
Console.WriteLine("Modified contrast: " + picture.FormatPicture.Contrast);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
