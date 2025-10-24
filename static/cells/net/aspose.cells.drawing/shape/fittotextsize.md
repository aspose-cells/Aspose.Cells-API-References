##Shape.FitToTextSize
Shape method. Recalculate a text area suitable for displaying all text content
## Shape.FitToTextSize method
Recalculate a text area suitable for displaying all text content.
```csharp
public void FitToTextSize()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeMethodFitToTextSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";
try
{
// Display original dimensions
Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");
// Call the FitToTextSize method
textBox.FitToTextSize();
// Display adjusted dimensions
Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
Console.WriteLine("FitToTextSize method executed successfully");
// Add more text to show the effect
textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
textBox.FitToTextSize();
Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
}
// Save the result
workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
