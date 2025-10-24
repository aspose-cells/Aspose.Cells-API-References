##Shape.GetRichFormattings
Shape method. Returns all Characters objects that represents a range of characters within the text
## Shape.GetRichFormattings method
Returns all Characters objects that represents a range of characters within the text .
```csharp
public FontSetting[] GetRichFormattings()
```
### Return Value
All Characters objects
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetRichFormattingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with rich text (correct parameter count for AddRectangle)
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
shape.Text = "This is bold and this is italic";
// Format parts of the text
shape.Characters(0, 4).Font.IsBold = true;
shape.Characters(13, 6).Font.IsItalic = true;
// Get rich text formattings
FontSetting[] formattings = shape.GetRichFormattings();
// Display formatting information
Console.WriteLine("Rich text formattings:");
foreach (FontSetting setting in formattings)
{
Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
Console.WriteLine($"Start index: {setting.StartIndex}");
Console.WriteLine($"Length: {setting.Length}");
Console.WriteLine($"Bold: {setting.Font.IsBold}");
Console.WriteLine($"Italic: {setting.Font.IsItalic}");
Console.WriteLine();
}
}
}
}
```
### See Also
* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
