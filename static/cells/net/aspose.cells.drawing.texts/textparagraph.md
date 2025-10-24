##Class TextParagraph
Aspose.Cells.Drawing.Texts.TextParagraph class. Represents the text paragraph setting
## TextParagraph class
Represents the text paragraph setting.
```csharp
public class TextParagraph : FontSetting
```
## Properties
| Name | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Gets and sets the text horizontal alignment type of the paragraph. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Gets the bullet. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Gets and sets the default size for a tab character within this paragraph. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Specifies the left margin of the paragraph. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Specifies the right margin of the paragraph. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Gets tab stop list. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Gets the type of text node. |
## Methods
| Name | Description |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Sets the preset WordArt style.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextsClassTextParagraphDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a text box to the worksheet
int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
// Set text content with multiple paragraphs
textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";
// Access and modify text paragraphs
foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
{
// Set paragraph properties
paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
paragraph.LineSpace = 20;
paragraph.AlignmentType = TextAlignmentType.Center;
}
// Save the workbook
workbook.Save("TextParagraphDemo.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
