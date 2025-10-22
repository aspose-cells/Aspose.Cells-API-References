##TextParagraph.AlignmentType
TextParagraph property. Gets and sets the text horizontal alignment type of the paragraph
## TextParagraph.AlignmentType property
Gets and sets the text horizontal alignment type of the paragraph.
```csharp
public TextAlignmentType AlignmentType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertyAlignmentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
textBox.Text = "First Line\nSecond Line\nThird Line";
// Get the text paragraphs
TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
// Set different alignment for each paragraph
paragraphs[0].AlignmentType = TextAlignmentType.Center;
paragraphs[1].AlignmentType = TextAlignmentType.Left;
paragraphs[2].AlignmentType = TextAlignmentType.Right;
// Save the workbook
workbook.Save("TextParagraphAlignmentDemo.xlsx");
Console.WriteLine("Text paragraph alignment demo completed successfully.");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
