##ShapeCollection.AddOleObject
ShapeCollection method. Adds an OleObject
## ShapeCollection.AddOleObject method
Adds an OleObject.
```csharp
public OleObject AddOleObject(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width, byte[] imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 |  |
| top | Int32 |  |
| upperLeftColumn | Int32 |  |
| left | Int32 |  |
| height | Int32 |  |
| width | Int32 |  |
| imageData | Byte[] |  |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddOleObjectWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
byte[] imageData = File.ReadAllBytes("image.jpg");
shapes.AddOleObject(4, 0, 5, 0, 300, 500, imageData);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
