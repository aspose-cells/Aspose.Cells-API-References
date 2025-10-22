##TextParagraph.LeftMargin
TextParagraph property. Specifies the left margin of the paragraph
## TextParagraph.LeftMargin property
Specifies the left margin of the paragraph.
```csharp
public double LeftMargin { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyLeftMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";
// Get the text paragraph from the text box's first paragraph
TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
// Display the current left margin value
Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);
// Set a new left margin value (in points)
paragraph.LeftMargin = 20.0;
// Demonstrate the effect by adding another text box with default margin
TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
textBox2.Text = "This text box has default left margin.\nCompare the indentation.";
// Save the workbook to show the difference
workbook.Save("TextParagraphLeftMarginDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
