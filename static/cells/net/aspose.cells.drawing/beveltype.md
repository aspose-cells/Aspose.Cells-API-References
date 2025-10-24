##Enum BevelType
Aspose.Cells.Drawing.BevelType enum. Represents a preset for a type of bevel which can be applied to a shape in 3D
## BevelType enumeration
Represents a preset for a type of bevel which can be applied to a shape in 3D.
```csharp
public enum BevelType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No bevel |
| Angle | `1` | Angle |
| ArtDeco | `2` | Art deco |
| Circle | `3` | Circle |
| Convex | `4` | Convex |
| CoolSlant | `5` | Cool slant |
| Cross | `6` | Cross |
| Divot | `7` | Divot |
| HardEdge | `8` | Hard edge |
| RelaxedInset | `9` | Relaxed inset |
| Riblet | `10` | Riblet |
| Slope | `11` | Slope |
| SoftRound | `12` | Soft round |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class BevelTypeDemo
{
public static void BevelTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);
// Access the 3D format of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Set the top bevel type and dimensions
threeDFormat.TopBevelType = BevelType.SoftRound;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
// Set the bottom bevel type and dimensions
threeDFormat.BottomBevelType = BevelType.Divot;
threeDFormat.BottomBevelWidth = 5;
threeDFormat.BottomBevelHeight = 5;
// Save the workbook
workbook.Save("BevelTypeExample.xlsx");
workbook.Save("BevelTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
