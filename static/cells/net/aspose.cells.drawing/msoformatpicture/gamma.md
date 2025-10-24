##MsoFormatPicture.Gamma
MsoFormatPicture property. Represents gamma of the picture
## MsoFormatPicture.Gamma property
Represents gamma of the picture.
```csharp
public double Gamma { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyGammaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a picture to the worksheet (using a sample image path)
int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
Picture picture = sheet.Pictures[pictureIndex];
// Access the MsoFormatPicture object
MsoFormatPicture formatPicture = picture.FormatPicture;
// Set the Gamma property
formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment
// Save the workbook
workbook.Save("MsoFormatPictureGammaDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
