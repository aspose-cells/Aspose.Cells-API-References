##ShapeCollection.AddIcons
ShapeCollection method. Adds svg image
## ShapeCollection.AddIcons method
Adds svg image.
```csharp
public Picture AddIcons(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width, byte[] imageByteData, byte[] compatibleImageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | The horizontal offset of shape from its left column, in unit of pixel. |
| height | Int32 | The height of shape, in unit of pixel. |
| width | Int32 | The width of shape, in unit of pixel. |
| imageByteData | Byte[] | The image byte data. |
| compatibleImageData | Byte[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
// Create a sample icon file (in real usage, you would use an existing file)
string iconPath = "icon.svg";
File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");
// Add icon to worksheet
using (FileStream fs = new FileStream(iconPath, FileMode.Open))
{
int len = (int)fs.Length;
byte[] imageData = new byte[len];
fs.Read(imageData, 0, len);
Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
}
// Save the workbook
workbook.Save("output.xlsx");
// Clean up (optional)
File.Delete(iconPath);
}
}
}
```
### See Also
* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
