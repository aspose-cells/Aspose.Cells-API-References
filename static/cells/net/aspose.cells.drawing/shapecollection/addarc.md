##ShapeCollection.AddArc
ShapeCollection method. Adds a ArcShape to the worksheet
## ShapeCollection.AddArc method
Adds a ArcShape to the worksheet.
```csharp
public ArcShape AddArc(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ArcShape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ArcShape, in unit of pixel. |
| width | Int32 | Represents the width of ArcShape, in unit of pixel. |
### Return Value
A ArcShape object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
workbook.Save("AddArcDemo.xlsx");
}
}
}
```
### See Also
* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
