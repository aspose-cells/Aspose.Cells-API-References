##TextOptions.Kerning
TextOptions property. Specifies the minimum font size at which character kerning will occur for this text run
## TextOptions.Kerning property
Specifies the minimum font size at which character kerning will occur for this text run.
```csharp
public double Kerning { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextOptionsPropertyKerningDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text to demonstrate kerning
var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
shape.Text = "Kerning Demonstration Text";
// Get the TextOptions of the shape
TextOptions textOptions = shape.TextOptions;
// Display the current kerning value
Console.WriteLine("Current Kerning value: " + textOptions.Kerning);
// Set kerning to 12 points (minimum font size for kerning to occur)
textOptions.Kerning = 12;
// Set a larger font size to observe kerning effect
textOptions.Size = 24;
// Save the workbook to see the effect
workbook.Save("PropertyKerningDemo.xlsx");
// Create another shape with different kerning for comparison
var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
shape2.Text = "Comparison Text Without Kerning";
shape2.TextOptions.Size = 24;
shape2.TextOptions.Kerning = 0; // No kerning
// Save again with both examples
workbook.Save("PropertyKerningDemoWithComparison.xlsx");
}
}
}
```
### See Also
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
