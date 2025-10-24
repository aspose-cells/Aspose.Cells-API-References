##Shape.TextBody
Shape property. Gets and sets the setting of the shapes text
## Shape.TextBody property
Gets and sets the setting of the shape's text.
```csharp
public FontSettingCollection TextBody { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapePropertyTextBodyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
FontSettingCollection fontSettingCollection = shape.TextBody;
fontSettingCollection.Text = "This is a test.";
workbook.Save("ShapeTextBodyDemo.xlsx");
}
}
}
```
### See Also
* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
