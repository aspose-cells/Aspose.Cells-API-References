##TextParagraph.LineSpaceSizeType
TextParagraph property. Gets and sets the amount of vertical white space that will be used within a paragraph
## TextParagraph.LineSpaceSizeType property
Gets and sets the amount of vertical white space that will be used within a paragraph.
```csharp
public LineSpaceSizeType LineSpaceSizeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertyLineSpaceSizeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box and set text
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
shape.Text = "First line\nSecond line";
// Get the second paragraph
TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
TextParagraph paragraph = paragraphs[1];
// Set line spacing properties
paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
paragraph.LineSpace = 2;
paragraph.SpaceAfter = 3;
paragraph.SpaceBefore = 4;
// Save and output
workbook.Save("TextParagraphPropertyLineSpaceSizeTypeDemo_output.xlsx");
Console.WriteLine("Demo executed successfully. Output file created.");
}
}
}
```
### See Also
* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
