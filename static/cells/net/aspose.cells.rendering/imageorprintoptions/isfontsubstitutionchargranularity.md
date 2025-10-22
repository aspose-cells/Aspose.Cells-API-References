##ImageOrPrintOptions.IsFontSubstitutionCharGranularity
ImageOrPrintOptions property. Indicates whether to only substitute the font of character when the cell font is not compatibility for it
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```
### Remarks
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Configure cell with potentially unsupported font
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Text with unavailable font");
Style style = cell.GetStyle();
style.Font.Name = "NonExistentFont";
cell.SetStyle(style);
// Create image rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = ImageType.Png, // Namespace reference now valid
DefaultFont = "Arial",
CheckWorkbookDefaultFont = false
};
// Display and modify property value
Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
// Render with default setting
new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");
// Change property and render again
options.IsFontSubstitutionCharGranularity = true;
Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");
// Save workbook for reference
workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
