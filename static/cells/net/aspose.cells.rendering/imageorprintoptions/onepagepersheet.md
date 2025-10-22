##ImageOrPrintOptions.OnePagePerSheet
ImageOrPrintOptions property. If OnePagePerSheet is true  all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
## ImageOrPrintOptions.OnePagePerSheet property
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
```csharp
public bool OnePagePerSheet { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyOnePagePerSheetDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Sample Data for OnePagePerSheet Demo");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Row " + i);
}
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.OnePagePerSheet = true; // Key property being demonstrated
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
// Create sheet render
SheetRender sr = new SheetRender(worksheet, options);
// Save the output image
sr.ToImage(0, "OnePagePerSheetOutput.png");
Console.WriteLine("Output saved with OnePagePerSheet=true");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
