##Enum PresetWordArtStyle
Aspose.Cells.Drawing.PresetWordArtStyle enum. Represents the preset WordArt styles
## PresetWordArtStyle enumeration
Represents the preset WordArt styles.
```csharp
public enum PresetWordArtStyle
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| WordArtStyle1 | `1` | Fill - Black, Text 1, Shadow |
| WordArtStyle2 | `2` | Fill - Blue, Accent 1, Shadow |
| WordArtStyle3 | `3` | Fill - Orange, Accent 2, Outline - Accent 2 |
| WordArtStyle4 | `4` | Fill - White, Outline - Accent 1, Shadow |
| WordArtStyle5 | `5` | Fill - Gold, Accent 4, Soft Bevel |
| WordArtStyle6 | `6` | Gradient Fill - Gray |
| WordArtStyle7 | `7` | Gradient Fill - Blue, Accent 1, Reflection |
| WordArtStyle8 | `8` | Gradient Fill - Gold, Accent 4, Outline - Accent 4 |
| WordArtStyle9 | `9` | Fill - White, Outline - Accent 1, Glow - Accent 1 |
| WordArtStyle10 | `10` | Fill - Gray-50%, Accent 3, Sharp Bevel |
| WordArtStyle11 | `11` | Fill - Black, Text 1, Outline - Background 1, Hard Shadow - Background 1 |
| WordArtStyle12 | `12` | Fill - Black, Text 1, Outline - Background 1, Hard Shadow - Accent 1 |
| WordArtStyle13 | `13` | Fill - Blue, Accent 1, Outline - Background 1, Hard Shadow - Accent 1 |
| WordArtStyle14 | `14` | Fill - White, Outline - Accent 2, Hard Shadow - Accent 2 |
| WordArtStyle15 | `15` | Fill - Gray-25%, Background 2, Inner Shadow |
| WordArtStyle16 | `16` | Pattern Fill - White, Text 2, Dark Upward Diagonal, Shadow |
| WordArtStyle17 | `17` | Pattern Fill - Gray-50%, Accent 3, Narrow Horizontal, Inner Shadow |
| WordArtStyle18 | `18` | Fill - Blue, Accent 1, 50%, Hard Shadow - Accent 1 |
| WordArtStyle19 | `19` | Pattern Fill - Blue, Accent 1, Light Downward Diagonal, Outline - Accent 1 |
| WordArtStyle20 | `20` | Pattern Fill - Blue-Gray, Text 2, Dark Upward Diagonal, Hard Shadow - Text 2 |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class PresetWordArtStyleDemo
{
public static void PresetWordArtStyleExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the shape collection of the worksheet
ShapeCollection shapes = worksheet.Shapes;
// Add a WordArt shape with a specific preset style
// Parameters: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
// Save the workbook
workbook.Save("PresetWordArtStyleExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
