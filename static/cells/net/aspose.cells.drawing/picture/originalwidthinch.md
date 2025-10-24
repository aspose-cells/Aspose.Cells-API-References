##Picture.OriginalWidthInch
Picture property. Gets the original width of picture in unit of inches
## Picture.OriginalWidthInch property
Gets the original width of picture, in unit of inches.
```csharp
public double OriginalWidthInch { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyOriginalWidthInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture (replace "example.jpg" with your actual image path)
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
Picture pic = worksheet.Pictures[imgIndex];
// Get and display original width in inches
double picWidthInch = pic.OriginalWidthInch;
Console.WriteLine($"Original picture width: {picWidthInch} inches");
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
