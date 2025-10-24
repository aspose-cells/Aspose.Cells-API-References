##Class StyleFlag
Aspose.Cells.StyleFlag class. Represents flags which indicates applied formatting properties
## StyleFlag class
Represents flags which indicates applied formatting properties.
```csharp
public class StyleFlag
```
## Constructors
| Name | Description |
| --- | --- |
| [StyleFlag](styleflag/)() | Constructs an object with all flags as false. |
## Properties
| Name | Description |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Alignment setting will be applied. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | All properties will be applied. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | All borders settings will be applied. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Bottom border settings will be applied. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Cell shading setting will be applied. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Diagonal down border settings will be applied. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Diagonal up border settings will be applied. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Font settings will be applied. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Font bold setting will be applied. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Font color setting will be applied. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Font italic setting will be applied. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Font name setting will be applied. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Font script setting will be applied. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Font size setting will be applied. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Font strikeout setting will be applied. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Font underline setting will be applied. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Hide formula setting will be applied. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Horizontal alignment setting will be applied. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Indent level setting will be applied. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Left border settings will be applied. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Locked setting will be applied. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Number format setting will be applied. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Hide formula setting will be applied. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Right border settings will be applied. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Rotation setting will be applied. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Shrink to fit setting will be applied. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Text direction setting will be applied. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Top border settings will be applied. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Vertical alignment setting will be applied. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Wrap text setting will be applied. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagDemo
{
public static void StyleFlagExample()
{
// Create a new workbook and get the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Header 1");
worksheet.Cells["B1"].PutValue("Header 2");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["B3"].PutValue(40);
// Create a new style object
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 12;
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.Yellow;
style.Pattern = BackgroundType.Solid;
// Create a new StyleFlag object
StyleFlag styleFlag = new StyleFlag
{
All = true,
Font = true,
FontSize = true,
FontBold = true,
CellShading = true
};
// Apply the style to a range of cells
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
range.ApplyStyle(style, styleFlag);
// Save the workbook
workbook.Save("StyleFlagExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
