##Picture.OriginalWidthCM
Picture property. Gets the original width of picture in unit of centimeters
## Picture.OriginalWidthCM property
Gets the original width of picture, in unit of centimeters.
```csharp
public double OriginalWidthCM { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyOriginalWidthCMDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Picture pic = worksheet.Pictures[imgIndex];
Console.WriteLine("Original width of the picture in centimeters: " + pic.OriginalWidthCM);
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
