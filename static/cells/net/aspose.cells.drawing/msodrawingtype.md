##Enum MsoDrawingType
Aspose.Cells.Drawing.MsoDrawingType enum. Represents office drawing objects type
## MsoDrawingType enumeration
Represents office drawing objects type.
```csharp
public enum MsoDrawingType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Group | `0` | Group |
| Line | `1` | Line |
| Rectangle | `2` | Rectangle |
| Oval | `3` | Oval |
| Arc | `4` | Arc |
| Chart | `5` | Chart |
| TextBox | `6` | TextBox |
| Button | `7` | Button |
| Picture | `8` | Picture |
| Polygon | `9` | Polygon |
| CheckBox | `11` | CheckBox |
| RadioButton | `12` | RadioButton |
| Label | `14` | Label |
| DialogBox | `15` | DialogBox |
| Spinner | `16` | Spinner |
| ScrollBar | `17` | ScrollBar |
| ListBox | `18` | ListBox |
| GroupBox | `19` | GroupBox |
| ComboBox | `20` | ComboBox |
| Comment | `25` | Comment |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | Only for preserving the drawing object in the template file. |
| Unknown | `29` | Only for preserving the drawing object in the xlsx file. |
| Slicer | `31` | Slicer |
| WebExtension | `32` | Web extension |
| SmartArt | `33` | Smart Art |
| CustomXml | `34` | Custom xml shape ,such as Ink. |
| Timeline | `35` | Timeline |
| Model3D | `36` | 3D Model |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class MsoDrawingTypeDemo
{
public static void MsoDrawingTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet
Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
rectangle.Name = "MyRectangle";
rectangle.AlternativeText = "This is a rectangle shape";
// Add an oval shape to the worksheet
Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
oval.Name = "MyOval";
oval.AlternativeText = "This is an oval shape";
// Add a line shape to the worksheet
Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
line.Name = "MyLine";
line.AlternativeText = "This is a line shape";
// Add a textbox shape to the worksheet
Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
textBox.Name = "MyTextBox";
textBox.AlternativeText = "This is a textbox shape";
textBox.Text = "Hello, Aspose.Cells!";
// Output the names and types of the shapes
foreach (Shape shape in worksheet.Shapes)
{
Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
}
// Save the workbook
workbook.Save("MsoDrawingTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
