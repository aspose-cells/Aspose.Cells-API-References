##ImageOrPrintOptions.CheckWorkbookDefaultFont
ImageOrPrintOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set this to true to try to use workbooks default font to show these characters first
## ImageOrPrintOptions.CheckWorkbookDefaultFont property
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.
```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```
### Remarks
Default is true.
### Examples
```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Sample Text");
// Set the default font for the workbook
workbook.DefaultStyle.Font.Name = "Arial";
workbook.DefaultStyle.Font.Size = 12;
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.OnePagePerSheet = true;
// Enable checking workbook default font
options.CheckWorkbookDefaultFont = true;
// Render the worksheet to image
SheetRender renderer = new SheetRender(sheet, options);
using (MemoryStream stream = new MemoryStream())
{
renderer.ToImage(0, stream);
// Save the image to file
using (FileStream file = new FileStream("output.png", FileMode.Create))
{
stream.WriteTo(file);
}
}
Console.WriteLine("Image generated with workbook default font check.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
