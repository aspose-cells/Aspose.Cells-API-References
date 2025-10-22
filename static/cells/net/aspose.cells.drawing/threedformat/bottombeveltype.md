##ThreeDFormat.BottomBevelType
ThreeDFormat property. Gets and sets the type of the bottom bevel or how far into the shape it is applied. In unit of Points
## ThreeDFormat.BottomBevelType property
Gets and sets the type of the bottom bevel, or how far into the shape it is applied. In unit of Points.
```csharp
public BevelType BottomBevelType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyBottomBevelTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.BottomBevelType = BevelType.Divot;
threeDFormat.BottomBevelWidth = 8;
threeDFormat.BottomBevelHeight = 8;
workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
}
}
}
```
### See Also
* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
