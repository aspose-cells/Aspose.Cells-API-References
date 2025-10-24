##Enum PresetShadowType
Aspose.Cells.Drawing.PresetShadowType enum. Represents preset shadow type
## PresetShadowType enumeration
Represents preset shadow type.
```csharp
public enum PresetShadowType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| NoShadow | `0` | No shadow. |
| Custom | `1` | Custom shadow. |
| OffsetDiagonalBottomRight | `2` | Outer shadow offset diagonal bottom right. |
| OffsetBottom | `3` | Outer shadow offset bottom. |
| OffsetDiagonalBottomLeft | `4` | Outer shadow offset diagonal bottom left. |
| OffsetRight | `5` | Outer shadow offset right. |
| OffsetCenter | `6` | Outer shadow offset center. |
| OffsetLeft | `7` | Outer shadow offset left. |
| OffsetDiagonalTopRight | `8` | Outer shadow offset diagonal top right. |
| OffsetTop | `9` | Outer shadow offset top. |
| OffsetDiagonalTopLeft | `10` | Outer shadow offset diagonal top left. |
| InsideDiagonalTopLeft | `11` | Inner shadow inside diagonal top Left. |
| InsideTop | `12` | Inner shadow inside top. |
| InsideDiagonalTopRight | `13` | Inner shadow inside diagonal top right. |
| InsideLeft | `14` | Inner shadow inside left. |
| InsideCenter | `15` | Inner shadow inside center. |
| InsideRight | `16` | Inner shadow inside right. |
| InsideDiagonalBottomLeft | `17` | Inner shadow inside diagonal bottom left. |
| InsideBottom | `18` | Inner shadow inside bottom. |
| InsideDiagonalBottomRight | `19` | Inner shadow inside diagonal bottom right. |
| PerspectiveDiagonalUpperLeft | `20` | Outer shadow perspective diagonal upper left. |
| PerspectiveDiagonalUpperRight | `21` | Outer shadow perspective diagonal upper right. |
| Below | `22` | Outer shadow below. |
| PerspectiveDiagonalLowerLeft | `23` | Outer shadow perspective diagonal lower left. |
| PerspectiveDiagonalLowerRight | `24` | Outer shadow perspective diagonal lower right. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassPresetShadowTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate shadow effects
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Set different preset shadow types
shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);
// Change to another shadow type
shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);
// Save the workbook
workbook.Save("PresetShadowTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
