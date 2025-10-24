##TextParagraph.RightMargin
TextParagraph property. Specifies the right margin of the paragraph
## TextParagraph.RightMargin property
Specifies the right margin of the paragraph.
```csharp
public double RightMargin { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyRightMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";
// Get the text paragraph from the text box's first paragraph
TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
// Display the current right margin value
Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);
// Set a new right margin value (in points)
paragraph.RightMargin = 20.0;
// Add another text box to show the difference
TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
textBox2.Text = "This text has default RightMargin for comparison.";
// Save the workbook to see the effect
workbook.Save("TextParagraphRightMarginDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
