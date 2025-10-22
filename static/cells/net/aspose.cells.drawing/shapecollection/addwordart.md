##ShapeCollection.AddWordArt
ShapeCollection method. Adds preset WordArt since Excel 2007.s
## ShapeCollection.AddWordArt method
Adds preset WordArt since Excel 2007.s
```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int upperLeftRow, int top,
int upperLeftColumn, int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | The preset WordArt Style. |
| text | String | The text. |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of shape, in unit of pixel. |
| width | Int32 | Represents the width of shape, in unit of pixel. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add a WordArt with specified parameters
Shape wordArt = shapes.AddWordArt(
PresetWordArtStyle.WordArtStyle1,
"Sample WordArt",
10,  // left
10,  // top
200, // width
50,  // height
100, // rotation
200  // z-order
);
// Save the workbook
workbook.Save("WordArtDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
