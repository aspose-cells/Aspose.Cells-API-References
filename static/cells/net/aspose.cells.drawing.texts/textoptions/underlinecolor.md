##TextOptions.UnderlineColor
TextOptions property. Gets or sets the color of underline
## TextOptions.UnderlineColor property
Gets or sets the color of underline.
```csharp
public CellsColor UnderlineColor { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextOptionsPropertyUnderlineColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text to demonstrate text options
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
shape.Text = "Underline Color Demo";
// Get the TextOptions from the shape
TextOptions textOptions = shape.TextOptions;
try
{
// Display current UnderlineColor value
CellsColor currentColor = textOptions.UnderlineColor;
Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");
// Set a new UnderlineColor (since property is read-write)
CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
newColor.Color = System.Drawing.Color.Red;
textOptions.UnderlineColor = newColor;
// Enable underline to see the effect
textOptions.Underline = FontUnderlineType.Single;
// Display the new UnderlineColor value
Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");
// Save the workbook to see the effect
workbook.Save("UnderlineColorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
