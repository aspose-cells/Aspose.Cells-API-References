##ThreeDFormat.BottomBevelWidth
ThreeDFormat property. Gets and sets the width of the bottom bevel or how far into the shape it is applied. In unit of Points
## ThreeDFormat.BottomBevelWidth property
Gets and sets the width of the bottom bevel, or how far into the shape it is applied. In unit of Points.
```csharp
public double BottomBevelWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyBottomBevelWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.BottomBevelType = BevelType.ArtDeco;
threeDFormat.BottomBevelWidth = 15;
threeDFormat.BottomBevelHeight = 8;
workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
