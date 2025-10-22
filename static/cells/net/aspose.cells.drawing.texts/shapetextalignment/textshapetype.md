##ShapeTextAlignment.TextShapeType
ShapeTextAlignment property. Gets and set the transform type of text
## ShapeTextAlignment.TextShapeType property
Gets and set the transform type of text.
```csharp
public AutoShapeType TextShapeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyTextShapeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
// Get the text alignment of the shape
ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;
// Set the TextShapeType property
shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
// Save the workbook
workbook.Save("TextShapeTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
