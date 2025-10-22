##MsoFormatPicture.TransparentColor
MsoFormatPicture property. Gets and sets the transparent color of the picture
## MsoFormatPicture.TransparentColor property
Gets and sets the transparent color of the picture.
```csharp
public CellsColor TransparentColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyTransparentColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample picture (using a solid color rectangle as example)
int pictureIndex = worksheet.Pictures.Add(0, 0, "sample.png");
Picture picture = worksheet.Pictures[pictureIndex];
// Set transparent color
CellsColor transparentColor = workbook.CreateCellsColor();
transparentColor.Color = Color.Blue;
picture.FormatPicture.TransparentColor = transparentColor;
// Get and display the transparent color
CellsColor currentTransparentColor = picture.FormatPicture.TransparentColor;
Console.WriteLine("Current transparent color: " + currentTransparentColor.Color);
// Save the workbook
workbook.Save("TransparentColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
