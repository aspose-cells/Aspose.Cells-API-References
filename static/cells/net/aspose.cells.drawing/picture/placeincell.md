##Picture.PlaceInCell
Picture method. Place this picture in the cell
## Picture.PlaceInCell method
Place this picture in the cell
```csharp
public void PlaceInCell()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PictureMethodPlaceInCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
Picture picture = worksheet.Pictures[pictureIndex];
// Place the picture in cell A1
picture.PlaceInCell();
// Verify the picture is placed in the cell
Cell cell = worksheet.Cells["A1"];
byte[] imageData = cell.EmbeddedImage;
Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
