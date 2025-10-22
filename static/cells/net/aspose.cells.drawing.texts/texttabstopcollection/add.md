##TextTabStopCollection.Add
TextTabStopCollection method. Adds a tab stop
## TextTabStopCollection.Add method
Adds a tab stop.
```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to add text with tab stops
var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
var textParagraph = shape.TextBody.TextParagraphs[0];
// Get the TextTabStopCollection
var tabStops = textParagraph.Stops;
try
{
// Call the Add method with TextTabAlignmentType.Left and position 50.0
int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
// Call the Add method with TextTabAlignmentType.Right and position 100.0
int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
// Add text with tabs to demonstrate the tab stops
shape.Text = "Left-aligned\tRight-aligned";
Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
}
}
}
```
### See Also
* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
