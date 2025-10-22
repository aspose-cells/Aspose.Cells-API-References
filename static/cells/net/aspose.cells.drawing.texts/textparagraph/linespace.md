##TextParagraph.LineSpace
TextParagraph property. Gets and sets the amount of vertical white space that will be used within a paragraph
## TextParagraph.LineSpace property
Gets and sets the amount of vertical white space that will be used within a paragraph.
```csharp
public double LineSpace { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertyLineSpaceDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
shape.Text = "First line\nSecond line";
// Access the text paragraphs
TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
// Configure line spacing for the second paragraph
TextParagraph paragraph = paragraphs[1];
paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
paragraph.LineSpace = 2; // Set line spacing to 2 points
// Save and reload to demonstrate persistence
string outputPath = "output_LineSpaceDemo.xlsx";
workbook.Save(outputPath);
// Reload to verify settings
Workbook loadedWorkbook = new Workbook(outputPath);
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
