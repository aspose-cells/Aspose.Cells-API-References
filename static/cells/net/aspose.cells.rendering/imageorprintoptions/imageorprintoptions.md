##ImageOrPrintOptions.ImageOrPrintOptions
ImageOrPrintOptions constructor. Ctor
## ImageOrPrintOptions constructor
Ctor.
```csharp
public ImageOrPrintOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Hello World!");
// Demonstrate #ctor usage
ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
imgOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
// Render the sheet to image
SheetRender sheetRender = new SheetRender(sheet, imgOptions);
sheetRender.ToImage(0, "output.png");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
