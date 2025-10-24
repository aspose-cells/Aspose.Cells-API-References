##ImageOrPrintOptions.TextCrossType
ImageOrPrintOptions property. Gets or sets displaying text type when the text width is larger than cell width
## ImageOrPrintOptions.TextCrossType property
Gets or sets displaying text type when the text width is larger than cell width.
```csharp
public TextCrossType TextCrossType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyTextCrossTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set long text that will exceed cell width
worksheet.Cells["A1"].PutValue("This is a long text that exceeds cell width");
worksheet.Cells["A1"].GetStyle().ShrinkToFit = false;
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
// Demonstrate different TextCrossType settings
options.TextCrossType = TextCrossType.Default;
SaveAsImage(workbook, options, "TextCrossType_Default.png");
options.TextCrossType = TextCrossType.CrossKeep;
SaveAsImage(workbook, options, "TextCrossType_CrossKeep.png");
options.TextCrossType = TextCrossType.CrossOverride;
SaveAsImage(workbook, options, "TextCrossType_CrossOverride.png");
options.TextCrossType = TextCrossType.StrictInCell;
SaveAsImage(workbook, options, "TextCrossType_StrictInCell.png");
}
private static void SaveAsImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
{
SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
sr.ToImage(0, fileName);
}
}
}
```
### See Also
* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
