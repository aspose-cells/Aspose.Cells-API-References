##TextParagraph.SpaceAfter
TextParagraph property. Gets and sets the amount of vertical white space that will be present after a paragraph
## TextParagraph.SpaceAfter property
Gets and sets the amount of vertical white space that will be present after a paragraph.
```csharp
public double SpaceAfter { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertySpaceAfterDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add text box and set text
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
shape.Text = "First paragraph\nSecond paragraph";
// Get paragraphs
TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
// Configure second paragraph spacing
TextParagraph p = paragraphs[1];
p.LineSpaceSizeType = LineSpaceSizeType.Points;
p.LineSpace = 2;
p.SpaceAfter = 3; // Demonstrate SpaceAfter property
p.SpaceBefore = 4;
// Save and verify
workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
// Reload to verify settings
Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
