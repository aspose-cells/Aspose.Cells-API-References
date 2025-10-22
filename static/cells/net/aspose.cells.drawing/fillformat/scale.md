##FillFormat.Scale
FillFormat property. Gets and sets the picture format scale
## FillFormat.Scale property
Gets and sets the picture format scale.
```csharp
public double Scale { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyScaleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
RectangleShape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
shape1.Fill.FillType = FillType.Texture;
shape1.Fill.Texture = TextureType.Denim;
shape1.Fill.Scale = 50;
RectangleShape shape2 = worksheet.Shapes.AddRectangle(0, 0, 2, 0, 100, 150);
shape2.Fill.FillType = FillType.Texture;
shape2.Fill.Texture = TextureType.Denim;
shape2.Fill.Scale = 150;
workbook.Save("FillFormatScaleDemo.xlsx");
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
