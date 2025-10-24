##TextBoxOptions.ShapeTextVerticalAlignment
TextBoxOptions property. It corresponds to Format Shape  Text Options  Text Box  Vertical Alignment in Excel
## TextBoxOptions.ShapeTextVerticalAlignment property
It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.
```csharp
public ShapeTextVerticalAlignmentType ShapeTextVerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyShapeTextVerticalAlignmentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 200, 400);
textBox.Text = "Vertical Alignment Example";
textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [ShapeTextVerticalAlignmentType](../../shapetextverticalalignmenttype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
