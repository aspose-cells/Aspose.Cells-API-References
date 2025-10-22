##ShapeCollection.AddLine
ShapeCollection method. Adds a LineShape to the worksheet
## ShapeCollection.AddLine method
Adds a LineShape to the worksheet.
```csharp
public LineShape AddLine(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of LineShape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of LineShape, in unit of pixel. |
| width | Int32 | Represents the width of LineShape, in unit of pixel. |
### Return Value
A LineShape object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddLineWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
