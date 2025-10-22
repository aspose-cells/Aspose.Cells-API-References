##TextParagraph.DefaultTabSize
TextParagraph property. Gets and sets the default size for a tab character within this paragraph
## TextParagraph.DefaultTabSize property
Gets and sets the default size for a tab character within this paragraph.
```csharp
public double DefaultTabSize { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyDefaultTabSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";
// Get the text paragraph from the text box's first paragraph
TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
// Display the current default tab size
Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);
// Set a smaller tab size (default is usually around 36 points)
paragraph.DefaultTabSize = 20.0;
Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);
// Add another text box with default tab size for comparison
TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";
// Save the workbook to see the difference in tab spacing
workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
