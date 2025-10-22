##TextParagraph.SpaceAfterSizeType
TextParagraph property. Gets and sets the amount of vertical white space that will be present after a paragraph
## TextParagraph.SpaceAfterSizeType property
Gets and sets the amount of vertical white space that will be present after a paragraph.
```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertySpaceAfterSizeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box and set text with multiple paragraphs
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
shape.Text = "First paragraph\nSecond paragraph";
// Get the second paragraph
TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
TextParagraph paragraph = paragraphs[1];
// Set space properties with size type
paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
paragraph.SpaceAfter = 10; // 10 points space after
// Save and reload to verify
string filePath = "TextParagraphPropertySpaceAfterSizeTypeDemo_Output.xlsx";
workbook.Save(filePath);
Workbook loadedWorkbook = new Workbook(filePath);
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
}
}
}
```
### See Also
* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
