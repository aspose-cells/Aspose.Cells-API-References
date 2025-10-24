##Shape.Characters
Shape method. Returns a Characters object that represents a range of characters within the text
## Shape.Characters method
Returns a Characters object that represents a range of characters within the text.
```csharp
public FontSetting Characters(int startIndex, int length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |
### Return Value
Characters object.
### Remarks
This method only works on shape with title.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodCharactersWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
shape.Text = "Sample Text";
// Get characters from index 0 with length 4
FontSetting fontSetting = shape.Characters(0, 4);
// Modify the font settings
fontSetting.Font.Color = System.Drawing.Color.Red;
fontSetting.Font.Size = 14;
fontSetting.Font.IsBold = true;
// Save the workbook
workbook.Save("ShapeCharactersDemo.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
