##Picture.OriginalHeightInch
Picture property. Gets the original height of picture in unit of inches
## Picture.OriginalHeightInch property
Gets the original height of picture, in unit of inches.
```csharp
public double OriginalHeightInch { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyOriginalHeightInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Picture pic = worksheet.Pictures[imgIndex];
Console.WriteLine("Original picture height in inches: " + pic.OriginalHeightInch);
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
