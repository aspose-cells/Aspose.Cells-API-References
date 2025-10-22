##ShapeCollection.AddShape
ShapeCollection method. Adds a Shape to the worksheet
## ShapeCollection.AddShape method
Adds a Shape to the worksheet.
```csharp
public Shape AddShape(MsoDrawingType type, int upperLeftRow, int top, int upperLeftColumn,
int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Mso drawing type. |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Shape, in unit of pixel. |
| width | Int32 | Represents the width of Shape, in unit of pixel. |
### Return Value
A Shape object.
### Remarks
The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddShapeWithMsoDrawingTypeInt32Int32Int32IDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
Shape shape = shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 200, 50);
Console.WriteLine("Shape added successfully.");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
