##Picture.ImageType
Picture property. Gets the image format of the picture
## Picture.ImageType property
Gets the image format of the picture.
```csharp
public ImageType ImageType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyImageTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Insert first picture (PNG)
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
Picture pic1 = worksheet.Pictures[imgIndex1];
Console.WriteLine("Picture 1 is of type: " + pic1.ImageType);
// Insert second picture (JPEG)
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
Picture pic2 = worksheet.Pictures[imgIndex2];
Console.WriteLine("Picture 2 is of type: " + pic2.ImageType);
}
}
}
```
### See Also
* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
