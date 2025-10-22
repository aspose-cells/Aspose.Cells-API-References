##ThreeDFormat.TopBevelHeight
ThreeDFormat property. Gets and sets the height of the top bevel or how far into the shape it is applied. In unit of Points
## ThreeDFormat.TopBevelHeight property
Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points.
```csharp
public double TopBevelHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyTopBevelHeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.TopBevelType = BevelType.Circle;
threeDFormat.TopBevelHeight = 15;
threeDFormat.TopBevelWidth = 10;
workbook.Save("ThreeDFormatTopBevelHeightDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
