##ImageOrPrintOptions.IsCellAutoFit
ImageOrPrintOptions property. Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false
## ImageOrPrintOptions.IsCellAutoFit property
Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false.
```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, this property is not used, please remove this property.. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample text that exceeds default column width
worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
// Create image rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Demonstrate IsCellAutoFit false (default)
Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
SaveAsImage(worksheet, options, "WithoutAutoFit.png");
// Change IsCellAutoFit to true
options.IsCellAutoFit = true;
Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
SaveAsImage(worksheet, options, "WithAutoFit.png");
Console.WriteLine("Images created successfully. Compare column widths in output files.");
}
private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
{
// Configure image format
options.ImageType = ImageType.Png;
// Render worksheet to image with specified options
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, fileName);
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
