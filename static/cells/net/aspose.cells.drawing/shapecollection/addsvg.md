##ShapeCollection.AddSvg
ShapeCollection method. Adds svg image
## ShapeCollection.AddSvg method
Adds svg image.
```csharp
public Picture AddSvg(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width, byte[] svgData, byte[] compatibleImageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | The horizontal offset of shape from its left column, in unit of pixel. |
| height | Int32 | The height of shape, in unit of pixel. |
| width | Int32 | The width of shape, in unit of pixel. |
| svgData | Byte[] | The svg image data. |
| compatibleImageData | Byte[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;
// Load SVG file
using (FileStream fs = new FileStream("image.svg", FileMode.Open))
{
int len = (int)fs.Length;
byte[] imageData = new byte[len];
fs.Read(imageData, 0, len);
// Add SVG to worksheet
Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
