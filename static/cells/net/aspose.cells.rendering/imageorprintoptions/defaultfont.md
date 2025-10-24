##ImageOrPrintOptions.DefaultFont
ImageOrPrintOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set Aspose.Cells will use system default font to show these unicode characters
## ImageOrPrintOptions.DefaultFont property
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.
```csharp
public string DefaultFont { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyDefaultFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample text to cell
worksheet.Cells["A1"].PutValue("Sample Text with Default Font");
// Create image options and set default font
ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
{
DefaultFont = "Arial", // Setting default font
ImageType = ImageType.Png
};
// Render worksheet to image
SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
sheetRender.ToImage(0, "output.png");
Console.WriteLine("Image generated with default font setting.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
