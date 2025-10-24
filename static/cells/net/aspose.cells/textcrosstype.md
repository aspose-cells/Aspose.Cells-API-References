##Enum TextCrossType
Aspose.Cells.TextCrossType enum. Enumerates displaying text type when the text width is larger than cell width
## TextCrossType enumeration
Enumerates displaying text type when the text width is larger than cell width.
```csharp
public enum TextCrossType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `1` | Display text like in Microsoft Excel. |
| CrossKeep | `2` | Display all the text by crossing other cells and keep text of crossed cells. |
| CrossOverride | `3` | Display all the text by crossing other cells and override text of crossed cells. |
| StrictInCell | `4` | Only display the text within the width of cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class CellsClassTextCrossTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample text in a cell that might overflow
worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.OnePagePerSheet = true;
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
// Demonstrate different TextCrossType settings
options.TextCrossType = TextCrossType.Default;
SaveToImage(workbook, options, "TextCrossType_Default.png");
options.TextCrossType = TextCrossType.CrossKeep;
SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
options.TextCrossType = TextCrossType.CrossOverride;
SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
options.TextCrossType = TextCrossType.StrictInCell;
SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
}
private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
{
SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
sr.ToImage(0, fileName);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
