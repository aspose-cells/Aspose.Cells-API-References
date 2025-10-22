##TextParagraph.Stops
TextParagraph property. Gets tab stop list
## TextParagraph.Stops property
Gets tab stop list.
```csharp
public TextTabStopCollection Stops { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyStopsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add text to a cell and get its text paragraph properties
worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
shape.Text = "Sample\tText\tWith\tTabs";
// Get the text paragraph
var textOptions = shape.TextBody.TextParagraphs[0];
// Display current tab stops count
Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);
// Add new tab stops
textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
textOptions.Stops.Add(TextTabAlignmentType.Right, 150);
// Display updated tab stops
Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
for (int i = 0; i < textOptions.Stops.Count; i++)
{
Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
}
// Save the workbook to see the effect
workbook.Save("TextParagraphStopsDemo.xlsx");
}
}
}
```
### See Also
* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
