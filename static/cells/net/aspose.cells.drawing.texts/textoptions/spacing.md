##TextOptions.Spacing
TextOptions property. Specifies the spacing between characters within a text run
## TextOptions.Spacing property
Specifies the spacing between characters within a text run.
```csharp
public double Spacing { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextOptionsPropertySpacingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
textBox.Text = "Sample Text with Spacing";
// Get the text options of the text box
TextOptions textOptions = textBox.TextOptions;
// Display the current spacing value
Console.WriteLine("Current Spacing value: " + textOptions.Spacing);
// Set new spacing values and see the effects
textOptions.Spacing = 2.0; // Increased spacing
Console.WriteLine("Text with increased spacing (2.0)");
// Save the workbook with first spacing
workbook.Save("TextSpacingDemo1.xlsx");
// Change spacing to negative value (characters closer together)
textOptions.Spacing = -1.0;
Console.WriteLine("Text with decreased spacing (-1.0)");
// Save the workbook with second spacing
workbook.Save("TextSpacingDemo2.xlsx");
// Reset to default spacing
textOptions.Spacing = 0.0;
Console.WriteLine("Text with default spacing (0.0)");
// Save the workbook with default spacing
workbook.Save("TextSpacingDemo3.xlsx");
}
}
}
```
### See Also
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
