##Shape.CalculateTextSize
Shape method. Recalculate the text area
## Shape.CalculateTextSize method
Recalculate the text area
```csharp
public int[] CalculateTextSize()
```
### Return Value
Text's Size in an array(width and height).
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodCalculateTextSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample text to cell A1
worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");
// Create a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);
// Set text to the shape
shape.Text = "This is a test string to calculate text size";
// Calculate the text size
int[] size = shape.CalculateTextSize();
// Output the results
Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
