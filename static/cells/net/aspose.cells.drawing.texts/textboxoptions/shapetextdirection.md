##TextBoxOptions.ShapeTextDirection
TextBoxOptions property. Gets or sets the text display direction within a given text body. It corresponds to Format Shape  Text Options  Text Box  Text direction in Excel
## TextBoxOptions.ShapeTextDirection property
Gets or sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel
```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyShapeTextDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
// Set text direction to vertical
shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
// Set some text to demonstrate the direction
shape.Text = "Vertical Text Example";
// Save the workbook
workbook.Save("TextBoxTextDirectionDemo.xlsx");
}
}
}
```
### See Also
* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
