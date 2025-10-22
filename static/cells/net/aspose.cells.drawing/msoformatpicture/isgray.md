##MsoFormatPicture.IsGray
MsoFormatPicture property. Indicates whether this picture should display in grayscale
## MsoFormatPicture.IsGray property
Indicates whether this picture should display in grayscale.
```csharp
public bool IsGray { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyIsGrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture shape
using (Stream imageStream = File.OpenRead("example.gif"))
{
Shape shape = worksheet.Shapes.AddPicture(0, 0, imageStream, 100, 100);
// Set picture format properties
shape.FormatPicture.Brightness = 90;
shape.FormatPicture.Contrast = 90;
shape.FormatPicture.IsGray = true;
// Save the workbook
workbook.Save("output.xlsx");
}
// Reload and verify the properties
Workbook loadedWorkbook = new Workbook("output.xlsx");
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
Console.WriteLine("Brightness: " + loadedShape.FormatPicture.Brightness);
Console.WriteLine("Contrast: " + loadedShape.FormatPicture.Contrast);
Console.WriteLine("IsGray: " + loadedShape.FormatPicture.IsGray);
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
