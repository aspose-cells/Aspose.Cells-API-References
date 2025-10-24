##Picture.OriginalWidth
Picture property. Gets the original width of the picture
## Picture.OriginalWidth property
Gets the original width of the picture.
```csharp
public int OriginalWidth { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyOriginalWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];
// Get and display the original width of the picture
int originalWidth = pic.OriginalWidth;
Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");
// Save the workbook
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
