##ImageOrPrintOptions.DefaultEditLanguage
ImageOrPrintOptions property. Gets or sets default edit language
## ImageOrPrintOptions.DefaultEditLanguage property
Gets or sets default edit language.
```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```
### Remarks
It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyDefaultEditLanguageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set the workbook's default font to one that supports CJK characters
workbook.DefaultStyle.Font.Name = "MS Gothic";
// Set Japanese text that will require proper wrapping
string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
sheet.Cells["A1"].Value = japaneseText;
// Configure cell formatting - fixed using correct property name
Cell cell = sheet.Cells["A1"];
Style style = cell.GetStyle();
style.IsTextWrapped = true;  // Correct property name for text wrapping
cell.SetStyle(style);
sheet.Cells.SetColumnWidth(0, 15);
sheet.Cells.SetRowHeight(0, 60);
// Create image rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.DefaultEditLanguage = DefaultEditLanguage.CJK;
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.CheckWorkbookDefaultFont = true;
// Render the worksheet to image
SheetRender renderer = new SheetRender(sheet, options);
renderer.ToImage(0, "CJK_Text_Rendering.png");
Console.WriteLine("Generated image with CJK text rendering.");
}
}
}
```
### See Also
* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
