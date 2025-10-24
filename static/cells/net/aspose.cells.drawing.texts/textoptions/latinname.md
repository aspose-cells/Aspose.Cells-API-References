##TextOptions.LatinName
TextOptions property. Gets and sets the latin name
## TextOptions.LatinName property
Gets and sets the latin name.
```csharp
public string LatinName { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextOptionsPropertyLatinNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate text options
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
shape.Text = "Sample Text";
// Get the TextOptions from the shape's first paragraph
TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;
// Display current LatinName value
Console.WriteLine("Current LatinName value: " + textOptions.LatinName);
// Set a new LatinName value
textOptions.LatinName = "Times New Roman";
// Create another shape to compare font rendering
Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
shape2.Text = "Comparison Text";
shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";
// Save the workbook to see the effects
workbook.Save("PropertyLatinNameDemo.xlsx");
// Display the new LatinName value
Console.WriteLine("New LatinName value: " + textOptions.LatinName);
}
}
}
```
### See Also
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
