##ShapeCollection.AddActiveXControl
ShapeCollection method. Creates an Activex Control
## ShapeCollection.AddActiveXControl method
Creates an Activex Control.
```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left,
int width, int height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ControlType | The type of the control. |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Shape, in unit of pixel. |
| width | Int32 | Represents the width of Shape, in unit of pixel. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
Shape activeXControl = shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox,
1,  // upperLeftRow
0,  // top
1,  // upperLeftColumn
0,  // left
100,  // width
50   // height
);
workbook.Save("AddActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
