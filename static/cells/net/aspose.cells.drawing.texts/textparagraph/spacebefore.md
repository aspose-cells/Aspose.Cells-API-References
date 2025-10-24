##TextParagraph.SpaceBefore
TextParagraph property. Gets and sets the amount of vertical white space that will be present before a paragraph
## TextParagraph.SpaceBefore property
Gets and sets the amount of vertical white space that will be present before a paragraph.
```csharp
public double SpaceBefore { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextParagraphPropertySpaceBeforeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add text box and set text
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
shape.Text = "First paragraph\nSecond paragraph";
// Get paragraphs
Aspose.Cells.Drawing.Texts.TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
// Configure second paragraph spacing
Aspose.Cells.Drawing.Texts.TextParagraph p = paragraphs[1];
p.LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Points;
p.LineSpace = 2;
p.SpaceAfter = 3;
p.SpaceBefore = 4; // Demonstrate SpaceBefore property
// Save and verify
string outputPath = "output_SpaceBeforeDemo.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Demo completed. File saved: " + outputPath);
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
