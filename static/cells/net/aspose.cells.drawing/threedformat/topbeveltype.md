##ThreeDFormat.TopBevelType
ThreeDFormat property. Gets and sets the type of the top bevel or how far into the shape it is applied. In unit of Points
## ThreeDFormat.TopBevelType property
Gets and sets the type of the top bevel, or how far into the shape it is applied. In unit of Points.
```csharp
public BevelType TopBevelType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyTopBevelTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.TopBevelType = BevelType.SoftRound;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
workbook.Save("ThreeDFormatTopBevelDemo.xlsx");
}
}
}
```
### See Also
* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
