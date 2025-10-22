##Shape.FormatPicture
Shape property. Gets and sets the options of the picture format
## Shape.FormatPicture property
Gets and sets the options of the picture format.
```csharp
public MsoFormatPicture FormatPicture { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyFormatPictureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[index];
// Access the shape's FormatPicture property
MsoFormatPicture msoFormatPicture = picture.FormatPicture;
// Modify picture format properties
msoFormatPicture.Brightness = 0.5f;
msoFormatPicture.Contrast = 0.7f;
msoFormatPicture.Transparency = 0.3f;
// Save the workbook
workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
