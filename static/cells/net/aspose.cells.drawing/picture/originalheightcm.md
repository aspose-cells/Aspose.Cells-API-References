##Picture.OriginalHeightCM
Picture property. Gets the original height of picture in unit of centimeters
## Picture.OriginalHeightCM property
Gets the original height of picture, in unit of centimeters.
```csharp
public double OriginalHeightCM { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyOriginalHeightCMDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Picture pic = worksheet.Pictures[imgIndex];
Console.WriteLine("Original height of the picture (cm): " + pic.OriginalHeightCM);
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
