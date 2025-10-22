##TextOptions.Fill
TextOptions property. Represents the fill format of the text
## TextOptions.Fill property
Represents the fill format of the text.
```csharp
public FillFormat Fill { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextOptionsPropertyFillDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
shape.Text = "Sample Text";
FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
TextOptions textOptions = fontSetting.TextOptions;
// Set font properties
textOptions.Name = "Arial";
textOptions.Size = 14;
textOptions.IsBold = true;
// Demonstrate Fill property
textOptions.Fill.FillType = FillType.Solid;
SolidFill solidFill = textOptions.Fill.SolidFill;
solidFill.Color = System.Drawing.Color.Blue;
// Save the workbook
workbook.Save("TextOptionsFillDemo.xlsx");
}
}
}
```
### See Also
* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
