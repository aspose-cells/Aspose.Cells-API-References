##Shape.TextBoxOptions
Shape property. Gets the text information in the shape
## Shape.TextBoxOptions property
Gets the text information in the shape
```csharp
public TextBoxOptions TextBoxOptions { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
public class ShapePropertyTextBoxOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
int textBoxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textBox = worksheet.TextBoxes[textBoxIndex];
textBox.Text = "This is a sample text box to demonstrate TextBoxOptions properties.";
// Display current TextBoxOptions properties
TextBoxOptions textBoxOptions = textBox.TextBoxOptions;
Console.WriteLine("Current TextBoxOptions:");
Console.WriteLine("Vertical Alignment: " + textBoxOptions.ShapeTextVerticalAlignment);
Console.WriteLine("Resize To Fit Text: " + textBoxOptions.ResizeToFitText);
Console.WriteLine("Text Direction: " + textBoxOptions.ShapeTextDirection);
Console.WriteLine("Left Margin: " + textBoxOptions.LeftMarginPt + " pt");
Console.WriteLine("Right Margin: " + textBoxOptions.RightMarginPt + " pt");
// Modify TextBoxOptions properties
textBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;
textBoxOptions.ResizeToFitText = true;
textBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
textBoxOptions.LeftMarginPt = 10;
textBoxOptions.RightMarginPt = 10;
textBoxOptions.TopMarginPt = 5;
textBoxOptions.BottomMarginPt = 5;
// Save the workbook
workbook.Save("TextBoxOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
