##TextParagraph.SpaceBeforeSizeType
TextParagraph property. Gets and sets the amount of vertical white space that will be present before a paragraph
## TextParagraph.SpaceBeforeSizeType property
Gets and sets the amount of vertical white space that will be present before a paragraph.
```csharp
public LineSpaceSizeType SpaceBeforeSizeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertySpaceBeforeSizeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box and get its shape
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
shape.Text = "First paragraph\nSecond paragraph";
// Access the second paragraph
TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
TextParagraph paragraph = paragraphs[1];
// Set paragraph spacing properties
paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
paragraph.SpaceBeforeSizeType = LineSpaceSizeType.Points;
paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
paragraph.LineSpace = 12;
paragraph.SpaceBefore = 8;
paragraph.SpaceAfter = 10;
// Save and reload to demonstrate persistence
string outputPath = "TextParagraphSpacingDemo.xlsx";
workbook.Save(outputPath);
// Reload to verify properties
Workbook loadedWorkbook = new Workbook(outputPath);
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
Console.WriteLine("SpaceBeforeSizeType: " + loadedParagraph.SpaceBeforeSizeType);
Console.WriteLine("SpaceBefore: " + loadedParagraph.SpaceBefore);
Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
Console.WriteLine("LineSpaceSizeType: " + loadedParagraph.LineSpaceSizeType);
Console.WriteLine("LineSpace: " + loadedParagraph.LineSpace);
}
}
}
```
### See Also
* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
