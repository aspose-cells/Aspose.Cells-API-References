##TextParagraph.Type
TextParagraph property. Gets the type of text node
## TextParagraph.Type property
Gets the type of text node.
```csharp
public override TextNodeType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet with all required parameters
var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
var textBody = textBox.TextBody;
textBody.Text = "Sample Text\nSecond Line";
// Get the first paragraph from the text body
var paragraphs = textBody.TextParagraphs;
TextParagraph paragraph = paragraphs[0];
// Display the current Type value
Console.WriteLine("Current TextNodeType: " + paragraph.Type);
// Demonstrate how the Type property affects behavior
if (paragraph.Type == TextNodeType.TextParagraph)
{
Console.WriteLine("This is a text paragraph node");
Console.WriteLine("You can access paragraph-specific properties like:");
Console.WriteLine("AlignmentType: " + paragraph.AlignmentType);
Console.WriteLine("LineSpace: " + paragraph.LineSpace);
}
else if (paragraph.Type == TextNodeType.TextRun)
{
Console.WriteLine("This is a simple text run node");
}
else if (paragraph.Type == TextNodeType.Equation)
{
Console.WriteLine("This is an equation node");
}
// Save the workbook
workbook.Save("TextParagraphPropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextNodeType](../../textnodetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
