##Enum FillType
Aspose.Cells.Drawing.FillType enum. Fill format type
## FillType enumeration
Fill format type.
```csharp
public enum FillType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Represents automatic formatting type. |
| None | `1` | Represents none formatting type. |
| Solid | `2` | Solid fill format. |
| Gradient | `3` | Gradient fill format. |
| Texture | `4` | Texture fill format(includes picture fill). |
| Pattern | `5` | Pattern fill format. |
| Group | `6` | Inherit the fill properties of the group. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassFillTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
// Set gradient fill type
rectangle.Fill.FillType = FillType.Gradient;
rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
// Add a text box
Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
textBox.Text = "Gradient Fill Example";
// Set gradient fill type for text box
textBox.Fill.FillType = FillType.Gradient;
textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);
// Save the workbook
workbook.Save("FillTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
