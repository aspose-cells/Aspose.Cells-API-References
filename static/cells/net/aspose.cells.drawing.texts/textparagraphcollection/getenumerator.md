##TextParagraphCollection.GetEnumerator
TextParagraphCollection method. Gets the enumerator of the paragraphs
## TextParagraphCollection.GetEnumerator method
Gets the enumerator of the paragraphs.
```csharp
public IEnumerator GetEnumerator()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
using System.Collections;
public class TextParagraphCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet with all required parameters
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";
// Get the text paragraphs collection
TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
try
{
// Call the GetEnumerator method
IEnumerator enumerator = paragraphs.GetEnumerator();
Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
Console.WriteLine("Paragraphs:");
// Iterate through the paragraphs using the enumerator
while (enumerator.MoveNext())
{
TextParagraph paragraph = (TextParagraph)enumerator.Current;
Console.WriteLine(textBox.Text); // Using the text from the textbox since TextParagraph doesn't have Text property
}
Console.WriteLine("Method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetEnumeratorDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
